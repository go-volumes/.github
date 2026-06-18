<p align="center"><img src="https://raw.githubusercontent.com/go-volumes/brand/main/social/go-volumes.png" alt="go-volumes" width="640"></p>

<h1 align="center">go-volumes</h1>
<p align="center">Pure-Go block storage — a copy-on-write volume pool plus pluggable backings. No cgo, no root.</p>
<p align="center">
  <a href="https://go-volumes.github.io/"><img src="https://img.shields.io/badge/website-go--volumes.github.io-0A6E96?style=flat-square&logo=githubpages&logoColor=white" alt="website"></a>
  <a href="https://go-volumes.github.io/docs/"><img src="https://img.shields.io/badge/docs-mkdocs--material-0A6E96?style=flat-square&logo=materialformkdocs&logoColor=white" alt="docs"></a>
  <img src="https://img.shields.io/badge/Go-1.26-00ADD8?style=flat-square&logo=go&logoColor=white">
  <img src="https://img.shields.io/badge/license-BSD--3--Clause-0A6E96?style=flat-square">
  <a href="https://github.com/go-filesystems"><img src="https://img.shields.io/badge/pairs%20with-go--filesystems-0079A8?style=flat-square"></a>
</p>

---

## What this is

`go-volumes` is a pure-Go block-storage stack — **no cgo, no root**. A
copy-on-write **pool** carves thin, snapshottable volumes out of shared storage;
a small **`Device` contract** lets any layer read and write them; and pluggable
**backings** decide where the bytes actually live — a local file, S3-compatible
object storage, or an immutable OCI artifact. Put a filesystem (e.g. via
[`go-filesystems`](https://github.com/go-filesystems)) on top.

## Repos

| Repo | |
|---|---|
| [`interface`](https://github.com/go-volumes/interface) | The block-device **`Device` contract** every layer reads and writes through — decoupling *where* the bytes live from the *format* on top. |
| [`pool`](https://github.com/go-volumes/pool) | The copy-on-write volume **pool** — snapshottable, reference-counted volumes that fail cleanly with `ErrPoolFull` instead of corrupting. A ZFS-inspired alternative to LVM thin provisioning. |
| [`s3`](https://github.com/go-volumes/s3) | An **S3-backed backing** — run a pool (or any block consumer) on S3-compatible object storage. From-scratch AWS SigV4, standard library only. |
| [`oci`](https://github.com/go-volumes/oci) | **Freeze** a volume into an immutable, content-addressed **OCI artifact** (chunk-deduped) and re-open it as a read-only backing. |

## Links

- 🌐 Website — <https://go-volumes.github.io/>
- 📖 Docs — <https://go-volumes.github.io/docs/>
- 🎨 Brand assets — <https://github.com/go-volumes/brand>

---
<p align="center"><sub>Branding in <a href="https://github.com/go-volumes/brand">go-volumes/brand</a>.</sub></p>
