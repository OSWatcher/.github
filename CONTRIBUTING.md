# Contributing to OSWatcher

Thanks for looking. OSWatcher is a multi-repository project, so the first question is usually *which* repository.

## Where does my change go?

| Change | Repository |
|---|---|
| Snapshot, diff or object-storage behaviour | [neogit](https://github.com/OSWatcher/neogit) |
| A new analysis or capture plugin | [oswatcher-plugins](https://github.com/OSWatcher/oswatcher-plugins) |
| Neo4j-side query procedures | [oswatcher-procedures](https://github.com/OSWatcher/oswatcher-procedures) |
| Image building, update chains, capture pipeline | [osw-builder](https://github.com/OSWatcher/osw-builder) |
| Compose stack, deployment, backup scripts | [oswatcher](https://github.com/OSWatcher/oswatcher) |
| API schema or resolvers | [graphql-api](https://github.com/OSWatcher/graphql-api) |
| Web interface | [frontend](https://github.com/OSWatcher/frontend) |
| Anything cross-cutting, or you are not sure | [oswatcher](https://github.com/OSWatcher/oswatcher) |

Writing a plugin is the lowest-friction way in: [oswatcher-plugins](https://github.com/OSWatcher/oswatcher-plugins) consumes an already-captured graph, so you do not need KVM, Packer or installation media to work on it.

## Before you start

Open an issue first for anything beyond a small fix. This is a solo-maintained project and it is much better to find out early that something is already in flight or heading a different direction.

## Pull requests

- Branch from the repository's default branch, and keep one logical change per PR.
- CI must be green. Each repository documents its own setup, generally Poetry for the Python repositories and npm for the TypeScript ones.
- Match the existing style. The Python repositories run black, flake8 and mypy.
- Add a test when you fix a bug or add behaviour.
- Write commit messages that explain why, not just what.

## Licensing

The active stack is Apache 2.0. By contributing you agree that your contribution is licensed under the same terms as the repository you are contributing to.

## Security

Do not report vulnerabilities in issues or pull requests. See [SECURITY.md](SECURITY.md).
