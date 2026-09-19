# SymonSaySource

What SyMoNeuRaL builds from. One branch per upstream family, tracking the source rather than
carrying it.

## Why this repository holds no source

The acquired trees are 22 GB. Putting them here would make every clone carry every upstream
whether or not it is being worked on, and would turn a licence question into an archaeology
problem. What matters for building from pristine source is not a copy of the bytes — it is
knowing exactly which bytes, and being able to prove it later:

- the commit, by full SHA, never a tag — a tag moves, a commit does not
- the licence as declared, with the checksum of the licence file itself
- the copyright line the licence obliges us to carry
- when it was acquired, and what state that acquisition is in
- the patches we apply, which are ours and are small

A tree can be re-fetched from those facts. The facts cannot be recovered from a tree.

## How it is laid out

| Branch | Holds |
|---|---|
| `main` | this index, and nothing else |
| one per family | the pins, licences and provenance for the components in that family |

A family matches the directory the source lives in on a build host, so a branch name and a
path are the same word. Where a family sits under another — storage under common, the engine
and the WebAssembly runtime under llm — the branch flattens the separator, because a name
cannot be both a branch and a directory of branches.

| Branch | Components | Licences declared |
|---|---|---|
| `adaptive-fabric` | 2 | unrecorded (2) |
| `api` | 16 | unrecorded (16) |
| `build` | 7 | unrecorded (7) |
| `build-stack` | 2 | unrecorded (2) |
| `cli` | 20 | unrecorded (20) |
| `common` | 24 | unrecorded (24) |
| `common-storage` | 1 | MIT (1) |
| `crypto` | 3 | unrecorded (3) |
| `diffuse` | 1 | unrecorded (1) |
| `live` | 1 | unrecorded (1) |
| `llm` | 4 | unrecorded (4) |
| `llm-engine` | 1 | MIT (1) |
| `llm-wasm` | 2 | MIT (2) |
| `platform` | 8 | unrecorded (8) |
| `ravencalc` | 12 | unrecorded (12) |
| `remix` | 1 | unrecorded (1) |
| `streamer` | 1 | unrecorded (1) |
| `web` | 2 | unrecorded (2) |

108 components tracked across 18 branches.

## Updating a source

1. Change the pin on that family's branch: new commit SHA, new date, new licence checksum if
   the licence file changed.
2. Say in the same commit what moved and why. A pin that changes without a reason recorded is
   a pin nobody can defend at a licence review.
3. If the licence changed, that is not a routine update. It is a decision, and it is recorded
   as one before the pin moves.

## What a pin looks like

```json
{
  "schema": "symoneural-acquisition/1",
  "component": "wasmer",
  "upstream_url": "https://github.com/wasmerio/wasmer",
  "commit_sha": "a6dc5e093e151cbc0647871a6be0ba8fc7259c11",
  "nearest_tag": "v7.4.0",
  "declared_license": "MIT",
  "license_md5": "71afdf3349f1efb1361cfd1e9e85bb8d",
  "copyright": "Copyright (c) 2019-present Wasmer, Inc. and its affiliates.",
  "acquired": "2026-09-18"
}
```

`nearest_tag` is written down for readers and is never what gets fetched.

## Rules that apply to every branch here

- **Acquired source is read-only.** Nothing is ever edited in place; a build exports a
  throwaway copy. A patch is a file on this branch, not an edit to somebody else's tree.
- **Nothing dated August 2026.** It predates the fresh start, and a pin that lands in it is <!-- gate-allow: no-august — states the rule, does not use an August artifact -->
  flagged rather than used.
- **No weights, in any format or size.**
- **A licence is recorded as declared, not as assumed.** The checksum is what makes that
  claim checkable a year later.

## The licence boundary

These four trees carry **two** licences between them, and that is the point of the split:

| Licence | Where | Why there |
|---|---|---|
| `SymonSaysLLC Proprietary License 1.0` | `SymonSayDistribute` | the product: source-available now, Apache-2.0 two years after each release |
| `SymonSaysLLC Proprietary License 1.0` | `SymonSayOSS`, `SymonSayOpen`, `SymonSaySource` | work meant to combine freely — with copyleft, with anyone's code, with itself |

Two rules follow, and they are not the same rule:

**A licence deviation inside a tree is a new branch.** If one component in a tree cannot carry
that tree's licence — an upstream obligation, a contributed file with its own terms — it gets
its own branch, and that branch states the licence at the top of its document. A tree stays
readable because every branch in it either carries the tree's licence or says plainly that it
does not.

**A genuinely third licence is a new tree.** If something needs terms that are neither of the
two above — a copyleft obligation on our own code, a third-party commercial licence, an
agreement with its own conditions — it does not go on a branch here. It becomes its own
repository at `/mnt/<repo>`, with its own index, because a tree whose licence you cannot state
in one line is a tree nobody can ship from.

Anything that fits none of the four is raised rather than guessed at, and work continues around
it instead of stopping on it.
