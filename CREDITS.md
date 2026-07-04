# Credits & Third-Party Licenses

Axiom Odyssey bundles third-party mods that make Minecraft 1.7.10 run on modern
Java (21–25). They are the work of their respective authors and are redistributed
here under the terms of their licenses. Full license texts are in
[`THIRD_PARTY_LICENSES/`](THIRD_PARTY_LICENSES/).

## Java 25 runtime core

### lwjgl3ify — v3.0.25
- Author: **GTNewHorizons**
- Source: https://github.com/GTNewHorizons/lwjgl3ify
- License: **GNU LGPL v3.0** → [`THIRD_PARTY_LICENSES/LGPL-3.0.txt`](THIRD_PARTY_LICENSES/LGPL-3.0.txt)
  (which incorporates the **GNU GPL v3.0** → [`THIRD_PARTY_LICENSES/GPL-3.0.txt`](THIRD_PARTY_LICENSES/GPL-3.0.txt))
- Bundled file: `minecraft/mods/lwjgl3ify-3.0.25.jar` plus the LWJGL3 launcher
  patches in `patches/` and the `mmc-pack.json` changes.

### UniMixins — v0.3.1 (unimixins-all-1.7.10-0.3.1)
- Author: **GTNewHorizons**
- Source: https://github.com/GTNewHorizons/UniMixins
- Main project license: **The Unlicense** (public domain)
  → [`THIRD_PARTY_LICENSES/Unlicense.txt`](THIRD_PARTY_LICENSES/Unlicense.txt)
- Bundled modules under their own licenses:
  - SpongeMixins — LGPL v3.0
  - MixinBooterLegacy — LGPL v2.1
  - GasStation — LGPL v3.0
  - GTNHMixins — LGPL v3.0
- Bundled file: `minecraft/mods/+unimixins-all-1.7.10-0.3.1.jar`

## LGPL compliance note

These libraries are shipped as standalone `.jar` files. Users may replace them
with a compatible modified version by swapping the jar in `minecraft/mods/`,
which satisfies the LGPL relinking requirement. Source code for each is available
at the GitHub links above.
