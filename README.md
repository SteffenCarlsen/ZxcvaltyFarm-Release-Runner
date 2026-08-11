# ZxcvaltyFarm Release Runner

This public repository contains only GitHub-hosted workflow code. The ZxcvaltyFarm and
Obfuckscator sources remain private and are checked out with separate read-only deploy keys.

The public runner exists because standard GitHub-hosted runners are free for public repositories.
It does not hold production signing keys or the offline root. The production server accepts a
release only after its root-owned verifier validates the exact runner repository, workflow, source
tag and commit, OIDC claims, release manifest, and artifact digests.

