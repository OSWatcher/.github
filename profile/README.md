# OSWatcher

> A queryable graph of how operating systems change, release over release.

OSWatcher builds VM images for historical operating system releases (Windows 95 through 11, Ubuntu 6.10 through 25.04), captures each image's filesystem and registry offline, and stores the result as a content-addressed Merkle graph in Neo4j. Think **git for golden images**, with the object graph in a database rather than a packfile, so you can ask which release first shipped a binary, every image that ever contained a given DLL, or how a registry subtree drifted across a decade of service packs.

Not to be confused with Oracle's OSWatcher Black Box (`oswbb`) metrics collector. This is offline image analysis, not runtime monitoring.

### 👉 Start at [**OSWatcher/oswatcher**](https://github.com/OSWatcher/oswatcher)

That repository explains the architecture and maps every other repository in reading order. If you would rather jump straight in:

| | |
|---|---|
| **Run the whole stack** | [oswatcher](https://github.com/OSWatcher/oswatcher) — Docker Compose, six services |
| **Understand the core idea** | [neogit](https://github.com/OSWatcher/neogit) — the snapshot and diff engine, `pipx install neogit` |
| **Capture your own images** | [osw-builder](https://github.com/OSWatcher/osw-builder) — the ISO-to-graph pipeline |

Apache 2.0 across the active stack. Solo-maintained, actively developed, APIs may still change.
