# Security Policy

## Reporting a vulnerability

Report vulnerabilities privately through GitHub's **Report a vulnerability** button, on the Security tab of the affected repository. That opens a private advisory visible only to the maintainer.

Please do not open a public issue for a security problem.

There is **no bug bounty**. This is a solo-maintained research project, so expect a first response within a couple of weeks rather than a couple of days.

## Scope

OSWatcher is offline analysis tooling for operating system images, not a hardened multi-tenant service. Two things are in scope and worth reporting:

- Vulnerabilities in the API, authentication or object-storage boundary of a deployment following the documented configuration.
- Escapes from the capture pipeline, which mounts and inspects untrusted disk images.

The following are known and **not** vulnerabilities:

- Blob download authentication and registry redaction ship **disabled by default** in the open-source configuration. This is a documented default, not a flaw. Review your configuration before exposing an instance publicly.
- Default credentials in `.env.example` files, which exist to be replaced.
- Findings against a deployment run with authentication disabled, which the local development setup does intentionally.

## Supported versions

Only the latest release of each component receives fixes. There are no long-term support branches.
