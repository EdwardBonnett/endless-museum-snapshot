# The Endless Museum Wikipedia snapshot

Offline English Wikipedia article data and a route graph for The Endless Museum.

The snapshot is dated 1 July 2026 and contains 7,315,936 articles. Download the snapshot and its installer from [Releases](https://github.com/EdwardBonnett/endless-museum-snapshot/releases). Downloads are split into parts of at most 1 GiB and verified with SHA-256 checksums.

With Python 3.9 or newer installed, download and install the data without a GitHub account:

```sh
curl -fL https://github.com/EdwardBonnett/endless-museum-snapshot/releases/download/data-2026-07-01-v1/download_data.py -o download_data.py
python3 download_data.py --project-dir ./museum-data
```

The files are installed in `museum-data/Snapshot`. To use an Unreal checkout, set `--project-dir` to its `unreal/EndlessMuseum` directory instead. Allow 20 GiB of free space during setup; the completed snapshot uses about 9.6 GiB. Rerun the command to resume interrupted downloads. Completed download parts are removed after verification and installation.

This repository distributes the Wikipedia snapshot. The game's source code and runtime asset bundle are maintained separately.

Article text is adapted and abridged from English Wikipedia contributors under [Creative Commons Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/). Formatting is changed and source material is abridged for museum rooms. Article titles are retained in the data; the corresponding pages on [English Wikipedia](https://en.wikipedia.org/) provide source material, contributors and revision histories. The game displays source links and credits for visited articles.

The Endless Museum is an independent project and is not affiliated with or endorsed by the Wikimedia Foundation.
