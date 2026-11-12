# Dusklight

A browser game: gather wisps, grab coloured power lights, light the four great beacons and carry the flame home, while rivals fight you for the light. Built with three.js, no build step.

## Run it

Open `index.html` through a web server (the models load with `fetch`, so double-clicking the file will not work):

    python3 -m http.server

then visit http://localhost:8000.

## Put it on GitHub Pages

1. Upload `index.html` and the `assets` folder to the root of the repository.
2. Settings > Pages > Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. The game appears at `https://<username>.github.io/<repository>/` after a minute or two.

## Levels

Single player runs a five-level campaign. Each level is unlocked by finishing the one before it.

1. **The Island** — Glimmerwood, graves, lake and embers. Fully built and play-tested end to end.
2. **The Desert** — Sunken temple, bone canyon, oasis and glass dunes. Fully built and play-tested end to end.
3. **The Ice Land** — Frozen lake, glacier pass, aurora fields.
4. **The Sky Garden** — Marble terraces, orchards, cloud rim.
5. **The War-zone Mansion** — Ruined estate, craters, burning ground.

Known gaps in levels 3 to 5: they share the Island's terrain shape and its four beacon positions, so the ground layout repeats across levels; their villains are recoloured player-hero models rather than distinct monsters; and the Sky Garden's floating islands are scenery you cannot walk on. Levels 3 to 5 load and play with no page errors, but only level 3 has been part-tested through its goals.

## Notes

- On GitHub the game is single-player against AI rivals. The live multiplayer room only works when the game is opened as a Claude artifact.
- three.js loads from a CDN, so the page needs an internet connection.
- Character models, all third-party assets with their own terms: `soldier.json`, `michelle.json` and `xbot.json` (three.js examples, originally Mixamo); `kade.json` (Ready Player Me sample avatar from the three.js examples); `varn.json` (Mixamo vampire from the LearnOpenGL repository); `nyx.json`, `kaida.json`, `thane.json`, `elyn.json`, `maldrin.json`, `vesper.json`, `goblin.json`, `demon.json`, `pip.json`, `nim.json`, `maw.json`, `skel.json` and `para.json` (Mixamo characters Arissa, Akai, Dreyar, Ely, Ganfaul, Eve, Goblin, Demon, Medea, Mutant, Maw, Skeleton Zombie and Parasite, via the tanish434/Mixamo-Animations-Characters mirror on Hugging Face, under Adobe's Mixamo terms). Check Adobe's Mixamo terms before redistributing these files publicly.

## Controls

WASD move, drag to look, click or Space to fire, E ability, P photo mode. Touch: joystick and on-screen buttons.
