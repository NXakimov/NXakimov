## Release & security maintainer

I am the second pair of eyes on [dtwinuz](https://github.com/dtwinuz) releases: I review and approve release pull requests for [bitg](https://github.com/dtwinuz/bitg), keep the supply chain checks green, and make sure every artifact can be verified by anyone.

[![OpenSSF Best Practices](https://www.bestpractices.dev/projects/16620/badge)](https://www.bestpractices.dev/projects/16620)
[![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/dtwinuz/bitg/badge)](https://scorecard.dev/viewer/?uri=github.com/dtwinuz/bitg)
[![Latest bitg release](https://img.shields.io/github/v/release/dtwinuz/bitg?label=bitg)](https://github.com/dtwinuz/bitg/releases/latest)

### What a release has to pass

| Gate | Why |
|---|---|
| Protected branch, required review, signed commits | No single person ships alone |
| CI and end-to-end tests on Windows, Linux and macOS | The input method is tested where it runs |
| Build provenance attestation (Sigstore) and SBOM (SPDX) | You can prove the file came from this repository's CI |
| Package manifests updated together (winget, Homebrew, Scoop, apt) | Every store gets the same version |

### Verify a bitg release yourself

```sh
gh release download v0.4.0 --repo dtwinuz/bitg --pattern '*.msi'
gh attestation verify bitg-0.4.0-x64.msi --repo dtwinuz/bitg
```

### Live

Updated daily by a GitHub Action in this repository.

<!-- live:start -->
<!-- live:end -->

---

Same person as [@XakimovNosirbek](https://github.com/XakimovNosirbek) · [xnosir.dtwin.uz](https://xnosir.dtwin.uz)
