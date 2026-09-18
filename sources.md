# build — source we build from

7 components. Pins are in `pins/`, one file per component.

This branch carries no upstream source. It carries what is needed to fetch exactly
the same source again and to defend that choice later: the commit, the declared licence,
and the checksum of the licence file itself.

| Component | State | Licence | Commit |
|---|---|---|---|
| `autoconf` | ACQUIRED | — | `44d712a26b0e` |
| `automake` | ACQUIRED | — | `e82d2d34d462` |
| `bitbake` | ACQUIRED | — | `046a90b0e9b7` |
| `libtool` | ACQUIRED | — | `309bb53a8adf` |
| `m4` | ACQUIRED | — | `fe2f13ab9ab9` |
| `ninja` | ACQUIRED | — | `3441b633c2fe` |
| `openembedded-core` | ACQUIRED | — | `fe7a24bc6711` |

## Licences declared here

| Licence | Components |
|---|---|
| — | 7 |

## Updating one of these

Change its pin, and say in the same commit what moved and why. A licence change is
not a routine update: it is a decision, recorded as one before the pin moves.

Nothing dated August 2026 may be used; a pin that lands in it is flagged rather than
built from. Acquired source is read-only — a patch is a file here, never an edit to
somebody else's tree.

The index of families is on `main`.
