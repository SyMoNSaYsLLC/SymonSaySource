# crypto — source we build from

3 components. Pins are in `pins/`, one file per component.

This branch carries no upstream source. It carries what is needed to fetch exactly
the same source again and to defend that choice later: the commit, the declared licence,
and the checksum of the licence file itself.

| Component | State | Licence | Commit |
|---|---|---|---|
| `stratum` | ACQUIRED | — | `c1a799139425` |
| `sv2-apps` | ACQUIRED | — | `d7d556d1a3c7` |
| `sv2-spec` | ACQUIRED | — | `67d2178e12b2` |

## Licences declared here

| Licence | Components |
|---|---|
| — | 3 |

## Updating one of these

Change its pin, and say in the same commit what moved and why. A licence change is
not a routine update: it is a decision, recorded as one before the pin moves.

Nothing dated August 2026 may be used; a pin that lands in it is flagged rather than
built from. Acquired source is read-only — a patch is a file here, never an edit to
somebody else's tree.

The index of families is on `main`.
