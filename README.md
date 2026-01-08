When creating a new Releases branch, we should always base it on the latest available release in the previous version line.

For example, even if the request says to create releases/26.1.0 from releases/25.4.0, we should first check whether a newer 25.4 release already exists. If releases/25.4.5.1 is available, that branch should be used as the source instead.

In short, always use the most recent release branch from the prior version when creating a new release branch.
