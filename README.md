# Human Music verdicts

Artists checked by Human Music's investigator, a research tool that judges
whether an artist's music is AI-generated. [Human Music](https://github.com/wai-lau/human-music),
a browser extension for YouTube Music and Spotify, downloads this list.

Each entry in `verdicts.json` has the artist's name, a verdict (`ai`, `human`
or `unsure`), a confidence from 0 to 100, and the artist's Spotify or YouTube
channel ID when known. The extension's filtering mode decides which
confidences block a song: Optimal blocks AI verdicts at 95 or more,
Aggressive at 60 or more.

`calibrated` turns true once the confidences have been checked against
artists known to be AI-generated and artists known to be people. Until then,
nothing on this list blocks anything.

A verdict is an estimate, not proof. If you think one is wrong, open an issue.

The investigator's code lives in
[wai-lau/human-music](https://github.com/wai-lau/human-music/tree/main/research/investigator).

MIT licensed.
