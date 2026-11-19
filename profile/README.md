# Ironflow

Agents and workflows need history that survives crashes, retries and short-lived machines. Ironflowx builds that layer in Rust: open, MIT-licensed, and usable piece by piece.

It is inspired by [Ironflow](https://ironflow.run). Ironflow 1.x, the shipping product, stays under the Ironflow License.

**Original author and architect of both projects:** [Altug Sahin](https://github.com/sahina)

![Layers: your agents and workflows sit on the ironflow engine (unreleased), which sits on the foundation crates (unreleased) and segment-log (0.1.0, released), which writes sealed history to disk. Dashed layers are in progress and not yet built on segment-log.](https://raw.githubusercontent.com/ironflowx/.github/main/profile/layers.svg)

| Project | What it is | Status |
| --- | --- | --- |
| [segment-log](https://github.com/ironflowx/segment-log) | Embedded append-only event log. Group commit: one fsync per batch of appends. Per-stream revisions, idempotency keys, seal. | [0.1.0](https://github.com/ironflowx/segment-log/releases/tag/v0.1.0) |
| [ironflow](https://github.com/ironflowx/ironflow) | Ironflow engine | Unreleased |
| [foundation](https://github.com/ironflowx/foundation) | Shared foundation crates | Unreleased |

All projects are MIT licensed. Issues and PRs welcome: see the [contributing guide](https://github.com/ironflowx/.github/blob/main/CONTRIBUTING.md). Report security problems privately as described in the [security policy](https://github.com/ironflowx/.github/blob/main/SECURITY.md).
