# Human Music verdicts

Lists that [Human Music](https://github.com/wai-lau/human-music), a browser
extension for YouTube Music and Spotify, downloads.

## verdicts.json

Artists that Human Music's investigator judged AI-generated. The
investigator is a research tool that checks artists no list knows yet. Only
AI verdicts are published here; the others stay private.

Each entry has the artist's name, a confidence from 0 to 100, and the
artist's Spotify or YouTube channel ID when known. The extension's filtering
mode decides which confidences block a song: Optimal blocks at 95 or more,
Aggressive at 60 or more.

`calibrated` turns true once the confidences have been checked against
artists known to be AI-generated and artists known to be people. Until then,
nothing on this list blocks anything.

A verdict is an estimate, not proof. If you think one is wrong, open an issue.

The investigator's code lives in
[wai-lau/human-music](https://github.com/wai-lau/human-music/tree/main/research/investigator).

## zoundhub.json

A daily copy of the clearest AI flags from [Zoundhub](https://zoundhub.com):
artists it rates 5 dots that also carry Deezer's AI label, with a debut in
2020 or later. Zoundhub calls its rating "an AI signal, not a verified
classification", so the less certain ratings are left out. A name that
Zoundhub also gives to a low-rated artist matches by Spotify ID only.

The data is Zoundhub's, not covered by this repository's licence. It is
refreshed once a day from the maintainer's computer
([scripts/zoundhub-refresh.sh](https://github.com/wai-lau/human-music/blob/main/scripts/zoundhub-refresh.sh)):
zoundhub.com doesn't answer requests from servers such as GitHub's.

## Licence

The verdicts and this repository's files are MIT licensed. `zoundhub.json`
holds Zoundhub's data.
