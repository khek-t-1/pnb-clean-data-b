# pnb-clean-data-b

Cleaned + exact-deduplicated pretrain and SFT data (derived from the `LLM-Pipeline-Resources` v1.0 bundle), split in 25 MiB parts.

This repo holds parts `145`–`288`; `pnb-clean-data-a` holds `000`–`144`.

Join and extract (after collecting all 289 parts from both repos):

```
cat cleandata.tar.*.part > cleandata.tar
sha256sum cleandata.tar    # expect cd5e72f486ac6882349314e0150eaf72f23a0f075da47d4e84df9624b2b23808
tar -xf cleandata.tar
```

Each upstream dataset keeps its own license; check before redistribution.
