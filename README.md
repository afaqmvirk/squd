# Squd music assets

Public, checksum-pinned song metadata and seek indexes used by Overlord Squd.
The website and Discord bot implementation remain in their existing private repository.
No credentials, Discord messages or applicant data are included here.

Download the two assets from [the pinned release](https://github.com/afaqmvirk/squd-music-assets/releases/tag/squd-discover-0eaecb5-v1):

- `catalog.sqlite.gz`: 39,832,381 bytes; a searchable catalog of 586,297 named MIDI files and 152,057 normalized title labels.
- `discover-index.bin`: 273,038,904 bytes; bounded-range access to 6,747,346 MIDI files in the upstream archive.

The exact URLs, sizes, SHA-256 checksums, seek points and dictionaries are described by `discover-manifest.json`. Verify downloads with `sha256sum -c SHA256SUMS`.
The full MIDI archive stays on the pinned Hugging Face dataset revision. No full source archive, original audio or lyrics are hosted here.

Derived metadata, index and seek dictionaries retain CC BY-NC-SA 4.0. See [NOTICE.md](NOTICE.md) for attribution, upstream licence and modifications. Composition and arrangement rights remain with their holders.
