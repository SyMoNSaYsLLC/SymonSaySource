# platform — source we build from

8 components. Pins are in `pins/`, one file per component.

This branch carries no upstream source. It carries what is needed to fetch exactly
the same source again and to defend that choice later: the commit, the declared licence,
and the checksum of the licence file itself.

| Component | State | Licence | Commit |
|---|---|---|---|
| `AWCC` | ACQUIRED | — | `0ec42c4b3ddc` |
| `glfw` | ACQUIRED | — | `d9d6f0f1f967` |
| `imgui` | ACQUIRED | — | `f1cc2ae15e53` |
| `json` | ACQUIRED | — | `55f93686c015` |
| `libusb-cmake` | ACQUIRED | — | `c8477c10ac2a` |
| `loguru` | ACQUIRED | — | `ba2240d19bae` |
| `open-gpu-kernel-modules` | ACQUIRED | — | `61dcc93722ec` |
| `stb` | ACQUIRED | — | `2c980bb59875` |

## Licences declared here

| Licence | Components |
|---|---|
| — | 8 |

## Updating one of these

Change its pin, and say in the same commit what moved and why. A licence change is
not a routine update: it is a decision, recorded as one before the pin moves.

Nothing dated August 2026 may be used; a pin that lands in it is flagged rather than <!-- gate-allow: no-august — states the rule, does not use an August artifact -->
built from. Acquired source is read-only — a patch is a file here, never an edit to
somebody else's tree.

The index of families is on `main`.
