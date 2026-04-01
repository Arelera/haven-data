# haven-data

Static official coverage-pack data for Haven.

This repo is intentionally simple:

- `official_pack_index.json` lists available downloadable packs.
- `packs/*.official-pack.json.gz` are the downloadable pack artifacts.
- `packs/*.official-pack.meta.json` are human-readable build metadata files.

The mobile app reads the index directly from:

- `https://raw.githubusercontent.com/Arelera/haven-data/main/official_pack_index.json`

And downloads pack artifacts from the URLs listed in that index.

No backend server is required. This repo is the public static host.
