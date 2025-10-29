Here are the detailed steps to troubleshoot the errors below:

Error 1:
I simply relocated the file to the first “appServer” directory and removed the extra “appServer ” folder.

Error 2:
This one is a bit tricky since the logs didn’t specify what the exact error was, so it took some time to figure out how to troubleshoot it. Usually, for this type of error, we can run the “Repair – Reconcile component database from blob store” task in Nexus to fix the issue. However, in this case, running the reconcile task alone isn’t enough to fully resolve the problem because it doesn’t completely refresh the blob metadata cache or rebuild the component indexes.

To work around this, I found that we can run a specific sequence of repair tasks that together achieve the same result:

Repair – Recalculate blob store storage: Forces Nexus to rescan the blob store and rebuild any missing .properties or metadata cache entries.

Repair – Reconcile component database from blob store: Re-synchronizes the database with the blob store.

Repair – Rebuild repository browse: Reconstructs the Browse tree in the UI so all components become visible again.

Repair – Rebuild Maven repository metadata (maven-metadata.xml): Regenerates the actual metadata files for each group and artifact.
