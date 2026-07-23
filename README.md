# Marigold Cross — Community Design Lab Prototype

A single-file, self-contained web prototype used to gather community input on
future healthcare technology for Marigold Cross, a fictional city designed
around the needs of South Asian communities in the UK.

Participants share a few optional details about themselves, pick a use case
(managing diabetes / supporting an older relative), choose their favourite
of three technology concepts, and talk through a short guided conversation
about it. At the end, a complete transcript of their session is downloaded
automatically as a `.txt` file.

## Live demo

Once published with GitHub Pages, your link will look like:

```
https://<your-username>.github.io/<repo-name>/
```

See **Deploying** below for the exact steps.

## Running it locally

No build step, no server, no dependencies. Just open the file in a browser:

1. Download or clone this repo
2. Double-click `index.html` (or right-click → Open with → your browser)

Everything — styling, logic, and all images — is embedded in the single
HTML file, so it also works completely offline.

## Deploying (GitHub Pages)

1. Create a new **public** GitHub repository
2. Upload `index.html` to the root of the repo and commit
3. Go to **Settings → Pages**
4. Under "Build and deployment", set **Source: Deploy from a branch**,
   **Branch: main**, folder **/ (root)**, then **Save**
5. Wait a minute, then refresh — GitHub will show your live URL at the top
   of the Pages settings screen

Any time you update the prototype, just re-upload `index.html` with the
same name — the live link doesn't change.

## What's inside

- Plain HTML/CSS/JavaScript — no frameworks, no build tooling
- All imagery is embedded as base64 data URIs, so the file is fully
  self-contained (no external image requests)
- Participant responses and the full conversation transcript are only ever
  handled in the browser and saved to the person's own downloads folder —
  nothing is sent to a server or stored remotely

## Notes for editors

- The whole app lives in one HTML file; open it in any text/code editor to
  make changes
- Because the file embeds large images as base64, it's a few MB in size —
  this is expected and well within GitHub's per-file limits
- There's no minification or build process, so edits take effect immediately
  on refresh
