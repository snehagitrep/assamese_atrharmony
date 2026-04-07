# website for sample audio

Template website for presenting Assamese ATR harmony examples from your paper.

## Repository structure

```text
.
├── index.html
└── assets
    ├── audio
    ├── waveforms
    ├── spectrograms
    ├── trajectories
    └── combined_figures
```

## Quick start (local preview)

1. Add your files under the `assets/` subfolders using the exact filenames referenced in `index.html`.
2. Run:

```bash
python3 -m http.server 8000
```

3. Open <http://localhost:8000>.

If you see a directory listing, confirm `index.html` exists in the folder where you started the server.

## GitHub Pages deployment

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Save and wait 1–2 minutes.

Your site URL will look like:

```text
https://<username>.github.io/<repo-name>/
```
