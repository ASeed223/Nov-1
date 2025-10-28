import org.sonatype.nexus.repository.storage.Query
import org.sonatype.nexus.repository.storage.StorageFacet

def repoName = 'EDRRELEASE'
def targetPath = 'gov/ca/ftb/arch/ecm/idax/IRSClientJar/maven-metadata.xml'

def repo = repository.repositoryManager.get(repoName)
def tx = repo.facet(StorageFacet).txSupplier().get()
tx.begin()
try {
  def q = Query.builder().where('name = ').param(targetPath).build()
  def hits = tx.findAssets(q, [repo]).toList()
  ['.md5', '.sha1'].each { suf ->
    hits.addAll(tx.findAssets(Query.builder().where('name = ').param(targetPath + suf).build(), [repo]).toList())
  }
  return hits.collect { [id: it.id(), name: it.name(), size: it.size()] }
} finally { tx.close() }
