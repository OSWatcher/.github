# 🕰️ OSWatcher

> A queryable graph of how operating systems change, release over release.

OSWatcher builds VM images for historical operating system releases (Windows 95 through 11, Ubuntu 6.10 through 25.04), captures each image's filesystem and registry offline, and stores the result as a content-addressed Merkle graph in Neo4j. Think **git for golden images**, with the object graph in a database rather than a packfile.

Ask it things like:

- 🔍 which release first shipped a given binary
- 🧬 every image that ever contained a specific DLL
- 📈 how a registry subtree drifted across a decade of service packs

### 👉 Start at [**OSWatcher/oswatcher**](https://github.com/OSWatcher/oswatcher)

That repository explains the architecture and maps every other repository in reading order.

⚖️ Apache 2.0 across the active stack · 🛠️ solo-maintained, actively developed, APIs may still change.
