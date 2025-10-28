{
  "name": "find_irsclientjar_metadata",
  "type": "groovy",
  "content": "import org.sonatype.nexus.repository.storage.Query\nimport org.sonatype.nexus.repository.storage.StorageFacet\n\nfinal String repoName = 'EDRRELEASE'\nfinal String targetPath = 'gov/ca/ftb/arch/ecm/idax/IRSClientJar/maven-metadata.xml'\n\ndef repo = repository.repositoryManager.get(repoName)\nif (repo == null) {\n  return [error: \"Repo not found: ${repoName}\"]\n}\n\ndef tx = repo.facet(StorageFacet).txSupplier().get()\ntx.begin()\ntry {\n  def hits = []\n  def q = Query.builder().where('name = ').param(targetPath).build()\n  hits.addAll(tx.findAssets(q, [repo]).toList())\n  ['.md5', '.sha1'].each { suf ->\n    hits.addAll(tx.findAssets(Query.builder().where('name = ').param(targetPath + suf).build(), [repo]).toList())\n  }\n  return hits.collect { a -> [id: a.id(), name: a.name(), size: a.size()] }\n} finally {\n  tx.close()\n}\n"
}
