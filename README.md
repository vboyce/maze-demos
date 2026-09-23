# maze-demos

Live demos of the Maze task in jsPsych: **https://vboyce.github.io/maze-demos/**

| Demo | What it shows |
|---|---|
| [Kid-friendly reading](https://vboyce.github.io/maze-demos/kid-maze-experiment/index.html) | Styled for children: guided practice, pictures, progress bar, pause/stop |
| [Targeted sentences with results](https://vboyce.github.io/maze-demos/moderate-experiment/index.html) | Attachment ambiguities in redo mode, then a graph of your RTs |
| [Target and filler sentences](https://vboyce.github.io/maze-demos/critical-experiment/index.html) | Maze Made Easy items without redo (a mistake ends the sentence) |
| [Short vignettes](https://vboyce.github.io/maze-demos/as-maze-experiment/index.html) | Altmann & Steedman (1988) multi-sentence items |
| [Natural Stories story](https://vboyce.github.io/maze-demos/ns-maze-experiment/index.html) | A Natural Stories passage |

No data from the demos is saved.

This repo only holds the **built** demos (`deploy/`); the GitHub Pages workflow (`.github/workflows/static.yml`) publishes `deploy/` on every push to `main`. The source is in [jspsych-maze](https://github.com/vboyce/jspsych-maze). To update a demo:

```sh
cd ../jspsych-maze/source
npm run build:kid-maze
unzip -o packaged/kid-maze-experiment_1.0.0.zip -d ../../maze-demos/deploy/
```

then commit and push here. Documentation: https://vboyce.github.io/maze-docs
