# api

The `api` branch of `SymonSaySource`.

§3.7: this is the map. Every directory below is listed with what lives there and
why a reader would go to it.

## Directories

| Directory | Holds |
|---|---|
| [`pins`](pins/pins.md) | what this branch builds from, by full SHA |

## api — source we build from

*Folded in from `sources.md` on 2026-09-20: §3.7 allows one
document per directory. Nothing was lost — the original file is at
`/home/google/Desktop/claude/quarantine-3.7-2026-09-20/mnt/SymonSaySource/api/sources.md`.*

16 components. Pins are in `pins/`, one file per component.

This branch carries no upstream source. It carries what is needed to fetch exactly
the same source again and to defend that choice later: the commit, the declared licence,
and the checksum of the licence file itself.

| Component | State | Licence | Commit |
|---|---|---|---|
| `annotated-doc` | ACQUIRED | — | `ef48d6ad51d2` |
| `annotated-types` | ACQUIRED | — | `9eb966801382` |
| `anyio` | ACQUIRED | — | `ffcd1542cd6d` |
| `certifi` | ACQUIRED | — | `f4bc676bc101` |
| `click` | ACQUIRED | — | `8b19813f2bfc` |
| `fastapi` | ACQUIRED | — | `95f8322ee1dc` |
| `h11` | ACQUIRED | — | `1c5b07581f05` |
| `httpcore` | ACQUIRED | — | `98209758cc14` |
| `httpx` | ACQUIRED | — | `26d48e0634e6` |
| `idna` | ACQUIRED | — | `03a9a11dd8ae` |
| `pydantic` | ACQUIRED | — | `001dea020e08` |
| `sniffio` | ACQUIRED | — | `ae020e13b98d` |
| `starlette` | ACQUIRED | — | `4f250d6b8145` |
| `typing-extensions` | ACQUIRED | — | `f29cd28d8ed7` |
| `typing-inspection` | ACQUIRED | — | `83d4dbb74fc3` |
| `uvicorn` | ACQUIRED | — | `8988c23704fc` |

## Licences declared here

| Licence | Components |
|---|---|
| — | 16 |

## Updating one of these

Change its pin, and say in the same commit what moved and why. A licence change is
not a routine update: it is a decision, recorded as one before the pin moves.

Nothing dated August 2026 may be used; a pin that lands in it is flagged rather than <!-- gate-allow: no-august — states the rule, does not use an August artifact -->
built from. Acquired source is read-only — a patch is a file here, never an edit to
somebody else's tree.

The index of families is on `main`.

## Where this leads

Into [`pins`](pins/pins.md).
