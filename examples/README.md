# Examples

Each file is a complete, reproducible build:

```bash
uv run signforge build --params examples/neon-classic.json -o out/open-neon
uv run signforge build --params examples/channel-bold.json -o out/cafe
uv run signforge build --params examples/mini-desk.json -o out/mini
uv run signforge build --params examples/halo-backlit.json -o out/halo
uv run signforge build --params examples/charge-replica.json -o out/charge  # the TEDx original
```

Or with artwork instead of text:

```bash
uv run signforge build --art your-logo.svg --style neon --cap-height 250 -o out/logo
```

Before printing a press-fit lens for the first time on YOUR printer/filament,
print the fit ladder and pick the value that snaps:

```bash
uv run signforge coupon -o out/coupons
```

## About `CHARGE.svg`

`CHARGE.svg` is the word-art from the author's own TEDxFargo CHARGE sign build
(the project this tool was extracted from — see
[tedxfargo-charge-sign](https://github.com/booherbg/tedxfargo-charge-sign)).
It ships here solely as the pipeline's ground-truth QA asset
(`scripts/qa_gold.py`, `tests/test_charge_parity.py`). It is not covered by
this repo's MIT license; don't reuse the artwork outside this test context.
