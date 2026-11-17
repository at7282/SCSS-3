# SCSS-3

This repository is a demonstration of decentralized source-code security enforcement with gittuf. It contains a gittuf root of trust, a signed policy, and a Reference State Log (RSL) that records branch updates. Commits and gittuf metadata are signed with Sigstore keyless identities.

The `main` branch is protected by a two-person approval rule with a threshold of two. The history also demonstrates compromise recovery: a malicious commit was recorded, its RSL entry was annotated as skipped, and a signed revert restored the last known-good tree. `hello.txt` and `feature.txt` are demonstration artifacts.
