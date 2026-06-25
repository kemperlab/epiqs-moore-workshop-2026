# EPiQS Moore Workshop 2026 — Website

A single-page static site for the EPiQS Moore Workshop (Bridging Quantum Materials and
Quantum Information), September 14–16, 2026, at NC State University, Raleigh, NC.

## Files
- `index.html` — the page (content lives here)
- `style.css` — styling

No build step. To preview locally, just open `index.html` in a browser, or run:

```
python3 -m http.server
```

then visit http://localhost:8000.

## Publishing to GitHub Pages

1. Create a new GitHub repository (e.g. `moore-workshop-2026`).
2. From this folder, push the files:
   ```
   git remote add origin https://github.com/<your-username>/moore-workshop-2026.git
   git branch -M main
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment**. Set **Source** to
   "Deploy from a branch", **Branch** to `main`, folder `/ (root)`, then **Save**.
4. The site goes live in a minute or two at
   `https://<your-username>.github.io/moore-workshop-2026/`.

### Optional: custom domain
Add a `CNAME` file containing your domain, and configure the DNS record per GitHub's
Pages documentation.

## Editing content
All names, affiliations, dates, goals, and topics are plain HTML in `index.html` —
edit them directly. The speaker and attendee lists are simple `<li>` items.
