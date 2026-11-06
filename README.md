# Squd music assets

Public, checksum-pinned song metadata and seek indexes used by Overlord Squd. The website and Discord bot implementation remain private. No credentials, Discord messages or applicant data are hosted here.

The `assets/` directory contains:

- `catalog.sqlite.gz`: 39,832,381 bytes, a searchable SQLite catalog of 586,297 named MIDI files and 152,057 normalized title labels.
- `index-000.bin` through `index-008.bin`: the 273,038,904-byte compressed seek index split into 32 MiB parts. Concatenating these parts restores the original index with SHA-256 `3a50ebe5b6fba4ea6baf0fdcbab21ee2b7246786e21784fcbd637be1479ef951`.
- `index-parts.json`: offsets, sizes and SHA-256 checksums of the parts.

Verify downloads with `sha256sum -c SHA256SUMS`. Runtime URLs use an immutable Git commit; HTTP byte ranges fetch only the compressed blocks needed for playback. The seek manifest is `discover-manifest.json`. The full MIDI archive stays on its pinned upstream Hugging Face revision.

Derived metadata, index and seek dictionaries retain CC BY-NC-SA 4.0. See [NOTICE.md](NOTICE.md) for attribution, upstream licence and modifications. Composition and arrangement rights remain with their holders. No original audio or lyrics are hosted here.
