# Security policy

## Reporting a vulnerability

Do not open a public issue for a security problem.

Report it privately through GitHub: open the affected repository, go to the **Security** tab, and click **Report a vulnerability**. Only the maintainers see the report.

Include what you can:

- the affected repository and commit or version
- what goes wrong, and what an attacker gains (for example data loss, corruption, or a crash)
- steps or a test case that reproduces it

We aim to acknowledge a report within 7 days and keep you updated until it is fixed. We credit reporters in the advisory unless you ask us not to.

## Supported versions

All projects are pre-1.0. Fixes land on the default branch and in the next release. Older releases do not get backports.

## Scope

Crash-safety and durability bugs count as security issues: a write that was acknowledged as durable but lost or corrupted after a crash, or a recovery that accepts a damaged file. Report them the same way.
