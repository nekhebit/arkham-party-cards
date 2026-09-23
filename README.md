# Arkham Party Cards

A single-page tool for Arkham Horror: The Card Game. Paste your party's
ArkhamDB deck links and get a combined list of how many copies of each
card the group needs.

No build step, no dependencies. It's one `index.html` file that calls the
[ArkhamDB public API](https://arkhamdb.com/api/) directly from the
browser.

## Usage

Open `index.html` (locally, or via GitHub Pages once deployed), paste one
deck link per line, and click Calculate.

Only **public decklists** work:
`https://arkhamdb.com/decklist/view/<id>/...`

Private "My Decks" links (`arkhamdb.com/deck/view/...`) require a login
that ArkhamDB won't grant to another site, so they'll fail. To include
one of those decks, publish it first (there's a "Publish" button on the
deck page in ArkhamDB), then use the resulting decklist link.

## Deploying to GitHub Pages

1. Push this folder to a GitHub repo.
2. In the repo, go to **Settings > Pages**.
3. Under "Build and deployment", set source to **Deploy from a branch**,
   pick the branch (e.g. `main`) and folder (`/ (root)` if this folder
   is the repo root, or `/docs` if you put it there).
4. Save. GitHub will publish the site at
   `https://<username>.github.io/<repo>/` within a minute or two.
