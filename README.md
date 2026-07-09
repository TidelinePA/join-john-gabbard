# Re-Elect Mayor John Gabbard — Campaign Website

A clean, modern, single-page campaign website for Mayor John Gabbard (Dana Point City Council). Built as static HTML/CSS/JS — no database or backend required, so it hosts free on GitHub Pages.

## Files

```
gabbard-site/
├── index.html          ← the entire website (HTML + CSS + JS in one file)
├── assets/
│   ├── logo-wordmark.png   ← "John Gabbard" navy/red logo (used in header)
│   ├── seal.png            ← round "Re-Elect" coastal seal (used in footer + favicon)
│   ├── john-hero.jpg       ← ADD THIS: John's portrait for the homepage hero
│   └── john-about.jpg      ← ADD THIS: a photo of John for the About section
└── README.md
```

## Add John's photos (2 minutes)

The site is already wired for two photos. Just save the image files into the `assets` folder with these exact names:

- `assets/john-hero.jpg` — best with the **vertical/portrait** shot (e.g. the seated photo). Shown in the homepage hero.
- `assets/john-about.jpg` — a **harbor / smiling** shot works well. Shown in the About section.

As soon as those files exist, the photos appear automatically. Until then, a styled placeholder shows in each spot. (JPG or PNG both work — if you use PNG, either rename it to `.jpg` or update the filename in `index.html`.)

## Things to customize before launch

Open `index.html` and search for these — each is marked with a comment:

1. **Donate link** — search for `id="donateBtn"`. Replace `href="#"` with your real donation page URL (Anedot, WinRed, etc.). The button opens in a new tab.
2. **Contact email** — search for `mailto:info@johngabbard.com` and swap in the real campaign email.
3. **Contact phone** — search for `tel:+19495550100` and the displayed `(949) 555-0100`; replace both with the real number.
4. **FPPC disclaimer** — search for `Paid for by Gabbard for Dana Point` and add your committee's FPPC ID number.
5. **Stats & bio** — the numbers in the stat strip and the About text are drawn from John's bio; edit any wording as you like.

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `gabbard-campaign`).
2. Upload the contents of this `gabbard-site` folder to the repo (so `index.html` sits at the repo root).
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Select branch **main** and folder **/ (root)**, then **Save**.
6. Wait ~1 minute. Your site will be live at `https://<your-username>.github.io/<repo-name>/`.

### Custom domain (optional)
To use a domain like `johngabbard.com`: in **Settings → Pages → Custom domain**, enter your domain and follow the DNS instructions. Add a file named `CNAME` (containing just your domain) to the repo root.

## Notes

- Fully responsive — works on phones, tablets, and desktop. Includes a mobile hamburger menu.
- Colors are pulled from the campaign logo (navy `#14284b`, red `#c8102e`) with a coastal accent.
- No cookies, tracking, or external dependencies except Google Fonts.
