# Hygge Massage Studio — Website

A single-page static website for Hygge Massage Studio (Emma Martin, LMT) in Portland, OR. All booking buttons link to the studio's MassageBook page.

Live details baked in:
- Address: 210 NW 17th Ave, Suite 201, Portland, OR 97209
- Phone: (503) 683-2213
- Services & pricing (Relaxation Reset, Tissue Issues, Full Body Tune-up)
- Hours (Mon 10–6, Fri–Sun by appointment, Tue–Thu closed)
- Booking URL: https://www.massagebook.com/therapists/hygge?src=external

## Design notes

The style is a hybrid of **Mediterranean Revival / stone monastery** and **Hygge-Scandinavian**:
- Warm limestone + aged plaster background tones
- Terracotta and candlelight (muted gold) accents
- Cormorant Garamond (serif) + Inter (sans) type pairing
- Subtle arched "cloister window" motifs on section dividers, service cards, and CTA
- Deep oak/shadow footer for a cozy, sheltered close

## Photos required

The HTML expects three image files sitting next to `index.html`. Save them with exactly these filenames:

- `building.jpg` — exterior of the Mediterranean Revival building (used as hero background)
- `lobby.jpg` — interior studio/lobby photo (used in "The Space" section)
- `emma.jpg` — portrait of Emma (used in the About section)

Any common format works — if your files are PNGs, rename the references in `index.html` (search for `.jpg`) or just rename the files to `.jpg`.

## Other things you may want to tweak

1. **Bio copy** — I wrote bio paragraphs for Emma in the About section based on the MassageBook profile. Replace with her own words if preferred.
2. **Reviews** — Three real MassageBook reviews are included in "Kind Words." Swap or add more as you like.

## Deploying to GitHub Pages

1. Create a new repository on GitHub (e.g. `hygge-site`).
2. Upload `index.html` and `README.md` to the repository (drag-and-drop in the web UI, or use git).
3. In the repo, go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
5. In a minute or two, your site will be live at `https://<your-username>.github.io/hygge-site/`.

### Command-line version

```bash
cd massage-site
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/<your-username>/hygge-site.git
git push -u origin main
```

Then enable Pages in the repo settings as above.

### Custom domain

If you want to use `hyggemassagestudio.com`:

1. In your DNS provider, add a CNAME record pointing to `<your-username>.github.io`.
2. Add a file named `CNAME` to the repo containing just `hyggemassagestudio.com`.
3. In **Settings → Pages**, enter the custom domain and enable HTTPS.

## Local preview

Double-click `index.html` to open it in a browser — no build step required.
