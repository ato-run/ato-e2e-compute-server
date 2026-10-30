# ato-e2e-compute-server
Immutable fixture: dynamic server (per-process nonce), no static output.
Used by S02-C (stays compute) and S02-G (static override must fail).

`formation/` contains a separately pinned `ato.capsule/1` route for the same
server behavior, for GitHub-source Formation acceptance. Its server accepts a
`PORT` override for local tests and defaults to 8080. The root Store manifest
and server remain unchanged for the S02 suite.
