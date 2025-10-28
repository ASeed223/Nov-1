{
  "name": "find_irsclientjar_metadata",
  "type": "groovy",
  "content": "def repoName = 'EDRRELEASE' \ndef targetPath = 'gov/ca/ftb/arch/ecm/idax/IRSClientJar/maven-metadata.xml' \n\ndef repo = repository.repositoryManager.get(repoName) \ndef storageFacetClass = Class.forName('org.sonatype.nexus.repository.storage.StorageFacet') \ndef tx = repo.facet(storageFacetClass).txSupplier().get() \n\ntx.begin() \ntry { \n  def bucket = tx.findBucket(repo) \n  def wanted = [targetPath, targetPath + '.md5', targetPath + '.sha1'] as Set \n  def hits = [] \n  for (def asset : tx.browseAssets(bucket)) { \n    if (wanted.contains(asset.name())) { \n      hits << [id: asset.id(), name: asset.name(), size: asset.size()] \n    } \n  } \n  return hits \n} finally { tx.close() }"
}
