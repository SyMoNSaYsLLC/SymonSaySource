# common — source we build from

24 components. Pins are in `pins/`, one file per component.

This branch carries no upstream source. It carries what is needed to fetch exactly
the same source again and to defend that choice later: the commit, the declared licence,
and the checksum of the licence file itself.

| Component | State | Licence | Commit |
|---|---|---|---|
| `accelerate` | ACQUIRED | — | `6afc1e5ee217` |
| `filelock` | ACQUIRED | — | `4efd93e0482e` |
| `fsspec` | ACQUIRED | — | `9e22b60ea6e9` |
| `hf-xet` | ACQUIRED | — | `de71453d952b` |
| `huggingface-hub` | ACQUIRED | — | `495b17c85296` |
| `jinja2` | ACQUIRED | — | `15206881c006` |
| `markdown-it-py` | ACQUIRED | — | `36c5f547144d` |
| `markupsafe` | ACQUIRED | — | `297fc8e356e6` |
| `mdurl` | ACQUIRED | — | `596bf1c8752d` |
| `networkx` | ACQUIRED | — | `7530809bfa1e` |
| `packaging` | ACQUIRED | — | `929fd4b1410a` |
| `psutil` | ACQUIRED | — | `9eea97dd6f1d` |
| `pygments` | ACQUIRED | — | `a43b45dcf081` |
| `pytorch` | ACQUIRED | — | `2b3ec3482903` |
| `pyyaml` | ACQUIRED | — | `49790e73684b` |
| `regex` | ACQUIRED | — | `7dd71c15c4fb` |
| `rich` | ACQUIRED | — | `6ac483cbea39` |
| `safetensors` | ACQUIRED | — | `a406ca3e7a90` |
| `setuptools` | ACQUIRED | — | `72e919a8b10a` |
| `shellingham` | ACQUIRED | — | `cba059e7f29f` |
| `tokenizers` | ACQUIRED | — | `88a4498ad4ea` |
| `tqdm` | ACQUIRED | — | `9cf5a12b1f95` |
| `transformers` | ACQUIRED | — | `856157a2f3e9` |
| `typer` | ACQUIRED | — | `99eb220df7c6` |

## Licences declared here

| Licence | Components |
|---|---|
| — | 24 |

## Updating one of these

Change its pin, and say in the same commit what moved and why. A licence change is
not a routine update: it is a decision, recorded as one before the pin moves.

Nothing dated August 2026 may be used; a pin that lands in it is flagged rather than <!-- gate-allow: no-august — states the rule, does not use an August artifact -->
built from. Acquired source is read-only — a patch is a file here, never an edit to
somebody else's tree.

The index of families is on `main`.
