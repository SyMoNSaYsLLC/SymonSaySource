# llm — source we build from

4 components. Pins are in `pins/`, one file per component.

This branch carries no upstream source. It carries what is needed to fetch exactly
the same source again and to defend that choice later: the commit, the declared licence,
and the checksum of the licence file itself.

| Component | State | Licence | Commit |
|---|---|---|---|
| `ggml` | ACQUIRED | — | `e91ded11bdcd` |
| `llama.cpp` | ACQUIRED | — | `5266f24da75d` |
| `triton` | ACQUIRED | — | `c01b6774b186` |
| `vllm` | ACQUIRED | — | `98dff2a81d74` |

## Licences declared here

| Licence | Components |
|---|---|
| — | 4 |

## Updating one of these

Change its pin, and say in the same commit what moved and why. A licence change is
not a routine update: it is a decision, recorded as one before the pin moves.

Nothing dated August 2026 may be used; a pin that lands in it is flagged rather than
built from. Acquired source is read-only — a patch is a file here, never an edit to
somebody else's tree.

The index of families is on `main`.
