# ravencalc — source we build from

12 components. Pins are in `pins/`, one file per component.

This branch carries no upstream source. It carries what is needed to fetch exactly
the same source again and to defend that choice later: the commit, the declared licence,
and the checksum of the licence file itself.

| Component | State | Licence | Commit |
|---|---|---|---|
| `cloudpickle` | ACQUIRED | — | `7576fff24b97` |
| `cython` | ACQUIRED | — | `ec152091ca7c` |
| `joblib` | ACQUIRED | — | `cd9a6b05fc4f` |
| `mpmath` | ACQUIRED | — | `b5c04506ef0c` |
| `narwhals` | ACQUIRED | — | `e34715d1e9e2` |
| `numpy` | ACQUIRED | — | `dd88c0c19b54` |
| `openblas` | ACQUIRED | — | `e0166008be8e` |
| `pybind11` | ACQUIRED | — | `d03662f0984f` |
| `scikit-learn` | ACQUIRED | — | `866c0f51e756` |
| `scipy` | ACQUIRED | — | `e4e854eaa8f1` |
| `sympy` | ACQUIRED | — | `16fa855354eb` |
| `threadpoolctl` | ACQUIRED | — | `d5bf10bcf90d` |

## Licences declared here

| Licence | Components |
|---|---|
| — | 12 |

## Updating one of these

Change its pin, and say in the same commit what moved and why. A licence change is
not a routine update: it is a decision, recorded as one before the pin moves.

Nothing dated August 2026 may be used; a pin that lands in it is flagged rather than <!-- gate-allow: no-august — states the rule, does not use an August artifact -->
built from. Acquired source is read-only — a patch is a file here, never an edit to
somebody else's tree.

The index of families is on `main`.
