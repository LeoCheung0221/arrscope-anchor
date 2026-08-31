# NarrScope Anchor Ledger

Public append-only anchor for [NarrScope](https://github.com/LeoCheung0221/NarrScope) observatory data integrity.

This repository stores **only cryptographic hashes** — never news content or private archive data.

## Files

| File | Purpose |
|------|---------|
| `anchors/anchors.jsonl` | Daily manifest `root` hash chain (append-only) |
| `anchors/latest.json` | Latest anchor for quick verification |

## Verify locally

```bash
curl -s https://raw.githubusercontent.com/LeoCheung0221/arrscope-anchor/main/anchors/latest.json
```

Each `root` corresponds to a row in the private observatory `manifest.jsonl`.
Git commit timestamp on this repo is the third-party anchor time.

## License

MIT — see LICENSE.
