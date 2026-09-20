# cli

The `cli` branch of `SymonSaySource`.

§3.7: this is the map. Every directory below is listed with what lives there and
why a reader would go to it.

## Directories

| Directory | Holds |
|---|---|
| [`pins`](pins/pins.md) | what this branch builds from, by full SHA |

## cli — source we build from

*Folded in from `sources.md` on 2026-09-20: §3.7 allows one
document per directory. Nothing was lost — the original file is at
`/home/google/Desktop/claude/quarantine-3.7-2026-09-20/mnt/SymonSaySource/cli/sources.md`.*

20 components. Pins are in `pins/`, one file per component.

This branch carries no upstream source. It carries what is needed to fetch exactly
the same source again and to defend that choice later: the commit, the declared licence,
and the checksum of the licence file itself.

| Component | State | Licence | Commit |
|---|---|---|---|
| `anthropic-sdk-python` | ACQUIRED | — | `eb21a4352015` |
| `anthropic-sdk-typescript` | ACQUIRED | — | `135f71e92976` |
| `attrs` | ACQUIRED | — | `7bfc49e9b22d` |
| `cffi` | ACQUIRED | — | `fd33e7700f0e` |
| `cryptography` | ACQUIRED | — | `ffde75a2b594` |
| `docstring-parser` | ACQUIRED | — | `87dca55a7b5b` |
| `httpx2` | ACQUIRED | — | `71ae23be5448` |
| `jiter` | ACQUIRED | — | `2b5ec63e505b` |
| `jsonschema` | ACQUIRED | — | `a7277432b0f7` |
| `jsonschema-specifications` | ACQUIRED | — | `3b846010c34c` |
| `opentelemetry-python` | ACQUIRED | — | `53a5a40c9604` |
| `pycparser` | ACQUIRED | — | `77de509f0268` |
| `pyjwt` | ACQUIRED | — | `c6fe464b356f` |
| `python-multipart` | ACQUIRED | — | `238ead62a0bb` |
| `python-sdk` | ACQUIRED | — | `9972c21aa420` |
| `referencing` | ACQUIRED | — | `944ed5a20bc5` |
| `rpds-py` | ACQUIRED | — | `7277eb681f6e` |
| `sse-starlette` | ACQUIRED | — | `6754ef387da9` |
| `truststore` | ACQUIRED | — | `0714f72a739d` |
| `typescript-sdk` | ACQUIRED | — | `cc4b41617ce3` |

## Licences declared here

| Licence | Components |
|---|---|
| — | 20 |

## Updating one of these

Change its pin, and say in the same commit what moved and why. A licence change is
not a routine update: it is a decision, recorded as one before the pin moves.

Nothing dated August 2026 may be used; a pin that lands in it is flagged rather than <!-- gate-allow: no-august — states the rule, does not use an August artifact -->
built from. Acquired source is read-only — a patch is a file here, never an edit to
somebody else's tree.

The index of families is on `main`.

## Where this leads

Into [`pins`](pins/pins.md).
