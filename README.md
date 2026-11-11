# ClusterVAD codebook demo

Audio demonstration for "ClusterVAD: Threshold-Free Unsupervised Voice Activity Detection with Pre-Trained Neural Representations".

Open the [demo](https://karlhajal.github.io/ClusterVAD/) to inspect the 100 clusters of the OLIVE-J layer-4 codebook, ordered by mean sonority on LJSpeech. Select a cluster to hear its decoded sustained run, synthesized centroid, and examples from the original audio.

The site contains the demonstration linked in the ARR submission at [demo-anon.github.io/ClusterVAD](https://demo-anon.github.io/ClusterVAD/). The interface and all 102 audio files are unchanged.

To serve the files locally with Python 3.11 or later and uv:

```sh
uv run --python 3.11 --no-project python -m http.server 8000
```

Open `http://localhost:8000`. The site uses static HTML, JavaScript, and WAV audio; it needs no build step. GitHub Pages serves the repository root from `main`.
