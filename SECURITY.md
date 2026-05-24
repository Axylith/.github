# Security policy

This policy applies to all repositories in the [Axylith](https://github.com/Axylith) organization.

## Reporting a vulnerability

If you find a security vulnerability in any Axylith project, please **do not open a public issue**.

Instead, report it privately through one of these channels:

- **GitHub Security Advisory:** preferred. Open a draft advisory at the affected repo's Security tab → "Report a vulnerability".
- **Email:** `security@axylith.com` (PGP key available on request).

Please include:

- The repository and version affected
- Steps to reproduce
- The impact you believe this has
- Any suggested mitigation

## What to expect

- **Within 72 hours:** acknowledgment that we received the report
- **Within 7 days:** initial assessment of severity and confirmation whether it's reproducible
- **Within 30 days:** patch released (for confirmed vulnerabilities) or detailed response explaining why not

Critical issues may move faster.

## Disclosure

We coordinate disclosure with reporters. The default is:

1. Patch ships in a new release
2. Advisory published with the release notes
3. Reporter credited (unless they prefer to remain anonymous)
4. CVE assigned if severity warrants

If a vulnerability is being actively exploited, we may release a patch immediately and publish the advisory at the same time.

## What's in scope

- Code in any public Axylith repository
- Build pipelines and CI configurations
- Documentation that, if followed, would compromise security

## What's out of scope

- Social engineering attacks against maintainers
- Denial of service via expected resource limits (e.g., uploading a 100GB file to a feature designed for documents)
- Vulnerabilities in third-party services we use (report those upstream)
- Issues requiring physical access to a developer's machine

## Bug bounty

There is currently no formal bug bounty program. Reports that lead to significant security improvements may receive a small token of appreciation (mention in release notes, organization swag if/when we have any). This is not a commitment.
