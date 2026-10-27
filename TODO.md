# openclaw-identyclaw-a2a-plugin — open work

> **Before editing:** Review [documentation-standard.md](https://github.com/discernible-io/docs/blob/main/docs/documentation-standard.md).

**Created:** 2026-10-27  
**Last reviewed:** 2026-10-27

Living backlog for this OpenClaw plugin (agents/plugins row in the [applicability matrix](https://github.com/discernible-io/docs/blob/main/docs/documentation-standard.md#applicability-matrix)). Full API cicd/config stack is N/A; coding, vocabulary, documentation, and TypeScript/publish gates from [`coding-standard.md`](https://github.com/discernible-io/docs/blob/main/docs/coding-standard.md) apply. Index: [`README.md`](README.md).

## Standards conformance gaps (host audit 2026-10-27)

| Gap | Standard | Evidence / action |
| --- | --- | --- |
| Missing root backlog (closed by this file) | documentation principle **21** | Index from README |
| Floating Actions | cicd pin rule / coding workflow | **Done 2026-10-27** — all workflow `uses:` SHA-pinned |
| Docs pointer | documentation / distribution | README is product-heavy; add a short reference to discernible-io/docs coding + vocabulary standards (reference-only) |
| Local `docs/` | distribution | Only `jwt-audience-alignment.md` — OK; do not treat as a standards tree |
| Runtime `console.*` | logging (when app logger exists) | ~12 `console.*` hits in `src/` — route through the plugin logger where one exists |
| Coding **PI 12** | coding | Keep `bun run check` / `typecheck` / coverage; record a coverage floor if `bun test --coverage` is retained; dry-run pack check already referenced as pattern |
| Workflow gates | coding workflow | Prefer `permissions: contents: read`, `persist-credentials: false`, and `timeout-minutes` on lint/test jobs |

## Suggested next order

1. SHA-pin Actions on the next workflow edit.
2. Index this `TODO.md` from README and link coding/vocabulary standards.
3. Reduce routine `console.*` in favor of structured logger calls.
