<p align="center"><img src="https://raw.githubusercontent.com/go-volumes/brand/main/social/go-volumes.png" alt="go-volumes" width="640"></p>

<h1 align="center">go-volumes</h1>
<p align="center">Pooled, copy-on-write volume management in pure Go — no cgo, no root.</p>
<p align="center">
  <a href="https://go-volumes.github.io/docs/"><img src="https://img.shields.io/badge/docs-mkdocs--material-0A6E96?style=flat-square&logo=materialformkdocs&logoColor=white" alt="docs"></a>
  <img src="https://img.shields.io/badge/Go-1.26-00ADD8?style=flat-square&logo=go&logoColor=white">
  <img src="https://img.shields.io/badge/license-MIT-0A6E96?style=flat-square">
  <a href="https://github.com/go-filesystems"><img src="https://img.shields.io/badge/pairs%20with-go--filesystems-0079A8?style=flat-square"></a>
</p>

---

## What this is

`go-volumes` is building a pooled, copy-on-write volume layer in pure Go:
carve thin, snapshottable volumes out of a shared pool, then put a filesystem
(e.g. via [`go-filesystems`](https://github.com/go-filesystems)) on top — all
without cgo or root.

## Repos

| | Repo | |
|---|---|---|
| <img src="https://raw.githubusercontent.com/go-volumes/brand/main/avatar/go-volumes-pool.png" width="36"> | [`pool`](https://github.com/go-volumes/pool) | The copy-on-write storage pool. |

## Links

- 📖 Docs — <https://go-volumes.github.io/docs/>
- 🎨 Brand assets — <https://github.com/go-volumes/brand>

---
<p align="center"><sub>Branding in <a href="https://github.com/go-volumes/brand">go-volumes/brand</a>.</sub></p>
