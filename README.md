# M. Saim Akram — portfolio

Static one-page site. Biography is locked to the resume. AI projects are the public repositories on github.com/SaimAkramGill.

Open `index.html` in a browser, or from this directory:

```bash
python -m http.server 8765
```

Then visit `http://127.0.0.1:8765`.

`PROJECT-SPEC.md` is the build contract, not a public page.

## Branches

`develop` is the working branch. A push or merge to `main` deploys the site to Netlify. Pushes to `develop` do not.

The production workflow is `.github/workflows/deploy-netlify.yml`. It needs two repository secrets:

- `NETLIFY_AUTH_TOKEN` — a Netlify personal access token
- `NETLIFY_SITE_ID` — the site API ID
