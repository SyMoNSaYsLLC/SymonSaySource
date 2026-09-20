# live

The `live` branch of `SymonSaySource`.

§3.7: this is the map. Every directory below is listed with what lives there and
why a reader would go to it.

## Directories

| Directory | Holds |
|---|---|
| [`pins`](pins/pins.md) | what this branch builds from, by full SHA |

## live — source we build from

*Folded in from `sources.md` on 2026-09-20: §3.7 allows one
document per directory. Nothing was lost — the original file is at
`/home/google/Desktop/claude/quarantine-3.7-2026-09-20/mnt/SymonSaySource/live/sources.md`.*

1 component. Pins are in `pins/`, one file per component.

This branch carries no upstream source. It carries what is needed to fetch exactly
the same source again and to defend that choice later: the commit, the declared licence,
and the checksum of the licence file itself.

| Component | State | Licence | Commit |
|---|---|---|---|
| `gstreamer` | ACQUIRED | — | `070125524a84` |

## Licences declared here

| Licence | Components |
|---|---|
| — | 1 |

## Updating one of these

Change its pin, and say in the same commit what moved and why. A licence change is
not a routine update: it is a decision, recorded as one before the pin moves.

Nothing dated August 2026 may be used; a pin that lands in it is flagged rather than <!-- gate-allow: no-august — states the rule, does not use an August artifact -->
built from. Acquired source is read-only — a patch is a file here, never an edit to
somebody else's tree.

The index of families is on `main`.

## Where this leads

Into [`pins`](pins/pins.md).
