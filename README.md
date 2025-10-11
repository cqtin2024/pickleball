# Pickleball - GitHub Pages + GitHub Actions Demo

This project demonstrates a static web app hosted on GitHub Pages that can safely request
GitHub Actions to update JSON data in the repository via `repository_dispatch`.

## How to use

1. Create a GitHub repository named `Pickleball` (or change the `repo` variable in `index.html`).
2. Upload all files and folders from this package to the `main` branch of the repo.
3. In GitHub, go to **Settings → Pages** and enable Pages from the `main` branch (root).
4. Create a Fine-grained Personal Access Token on GitHub with `Contents: Read and write` for your repo:
   - https://github.com/settings/tokens?type=fine-grained
5. Open the GitHub Pages site (URL shown in Pages settings), paste the token in the web UI, then add players.
6. Check `data/players.json` and commits in the repository.

Notes:
- Token is stored locally in browser `localStorage`.
- You can revoke the token at any time via GitHub settings.

