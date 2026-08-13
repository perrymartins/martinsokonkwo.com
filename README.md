# martinsokonkwo.com — site source

Static site (no build step). Files:

- `index.html` — the whole site (About, Ventures, Recognition, Press, Connect) plus schema.org `Person` structured data in a `<script type="application/ld+json">` block.
- `styles.css`
- `robots.txt`, `sitemap.xml` — currently point at the placeholder domain `martinsokonkwo.com`. Update every occurrence once you pick a real domain.
- `assets/` — put `headshot.jpg` here.

## Before you publish

1. **Pick a domain.** A domain matching your name (e.g. `martinsokonkwo.com` or `perrymartins.com`) is the single most useful thing for building an entity Google can recognize. Register through any registrar (Namecheap, Google Domains successor, etc.).
2. **Replace every `martinsokonkwo.com`** in `index.html`, `robots.txt`, and `sitemap.xml` with your actual domain, once chosen.

Done already: headshot is in `assets/headshot.jpg` (from "Martins-P-001-22.jpg", resized to 1200px/~115KB for fast loading) and wired into the hero section; Giglive.co is described in the Ventures section and linked throughout; the UK Companies House officer record (Gotright Limited, No. 16980018) and the book *Discover and Nurture Your Talents into a Successful Business* are cited in About, Ventures, Recognition, the new Book section, Press, and the JSON-LD (`birthDate`, `worksFor`, a separate `Book` schema block, and `sameAs`).

## Deploying

Any static host works. Two easy free options:

- **GitHub Pages**: push this folder to a GitHub repo, enable Pages in repo settings, point your domain's DNS at it via a `CNAME` file.
- **Netlify / Vercel**: drag-and-drop the folder in their dashboard, then attach your custom domain.

## After it's live — steps that actually move a Knowledge Panel

A site alone doesn't create a panel. These steps matter more:

1. **Verify the site in [Google Search Console](https://search.google.com/search-console)** and submit `sitemap.xml`, so Google indexes it.
2. **Keep your name identical everywhere** — this site, LinkedIn, Instagram, Facebook, and every press mention should use the same name/spelling ("Martins Okonkwo" / "Perry Martins") so Google can merge them into one entity.
3. **Get a Wikidata entry.** Wikidata is one of the strongest direct sources Knowledge Graph pulls from, and has a lower bar than Wikipedia (no strict notability requirement in the same way). Create one at wikidata.org citing the press articles you already have as sources.
4. **More independent (non-self-published) coverage helps most.** The Pulse, Tribune, Sun, Vanguard, and Nation articles you already have are good — more third-party profiles/interviews over time strengthen the entity further.
5. **Once a panel appears**, search your name on Google/mobile, look for "Claim this knowledge panel," and verify via Search Console or a linked social account.

This site's `sameAs` list in the JSON-LD is what ties your identity across LinkedIn, Instagram, Facebook, Gospelbuzz, and the press coverage — keep it updated as more sources appear.
