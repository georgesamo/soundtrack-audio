# soundtrack-audio

The pre-rendered soundtrack of [georgesamo.github.io](https://georgesamo.github.io/): 30-second MP3 pieces of every
track in every theme (`<theme>-<n>-<k>.mp3`, counted in `index.json`) and the phone player's full-length files
(`full/<theme>-<n>.mp3`). The music is written in the site's `assets/js/lofi.js`; these files are rendered and mastered
from it by soundtrack-lab's `publish-audio.sh`.

This repo is kept to **one commit**. Every publish replaces it (`ship-audio.sh` in soundtrack-lab amends and
force-pushes), so earlier renders are not kept anywhere. The site's deploy checks this repo out into its
`assets/audio/` before the build.
