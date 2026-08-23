# For You 💌

A one-page, pastel & cute site you can send to your girlfriend — envelope intro, love letter, countdown, photo gallery, and flip-card "reasons I love you."

**Files:**
- `index.html` — page structure & content
- `style.css` — all the styling (colors, layout, animations)

## 1. Customize it

Open `index.html` in any text editor and edit these spots:

| Find | Replace with |
|---|---|
| `{{GIRLFRIEND_NAME}}` (appears twice) | her name |
| `{{YOUR_NAME}}` | your name |
| the opening line inside `.letter-body` in `index.html` | already filled in with a suggested line — edit or replace with your own words freely |
| `reasons` array in the `<script>` at the bottom | your own list — any number of items works |

The countdown is already set to **September 25, 2026** (her birthday) — change the date in the `targetDate` line in `index.html` if needed.

A **✕ close** button sits under the signature so she can close the letter and go back to the envelope.

### Add real photos
Each `.photo-slot` div in the Gallery section is a placeholder. To use a real photo, replace one like this:

```html
<div class="photo-slot">
  <img src="photos/us1.jpg" alt="">
</div>
```

Create a `photos/` folder next to `index.html` and drop your images in there (`us1.jpg`, `us2.jpg`, etc.) — keep filenames simple, no spaces.

### Add a song (optional)
Put an mp3 file named `song.mp3` next to `index.html`, or change the `<source src="song.mp3">` line in the footer to match your filename. If you skip this, the play button will just prompt you to add one.

## 2. Deploy on GitHub Pages

1. Create a new GitHub repository (e.g. `for-her`).
2. Upload `index.html`, `style.css`, this `README.md`, and your `photos/` folder (and `song.mp3` if used) to the repo.
3. Go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
5. Wait a minute, then your site will be live at:
   `https://<your-username>.github.io/<repo-name>/`
6. Send her that link 💌

## Notes
- Just `index.html` + `style.css` (no build step, no dependencies besides Google Fonts) — keep them in the same folder.
- Respects reduced-motion settings and is keyboard-accessible (the envelope can be opened with Enter/Space).
