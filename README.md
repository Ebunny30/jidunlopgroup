# J.I. Dunlop Group — website

Single-page site. One `index.html` with all CSS and JS inline. No build step,
no frameworks, no dependencies except Google Fonts.

## Add the team photos

Drop these three files into this folder, next to `index.html`:

| File        | Person            |
|-------------|-------------------|
| `jonah.jpg` | Jonah Dunlop      |
| `james.jpg` | James Macdougall  |
| `tudor.jpg` | Tudor Panghe      |

The cards are 4:5 portrait. Around 1000 x 1250 px is ideal, but any portrait
photo works — they are cropped to fit automatically and never squashed.

Lowercase names with a lowercase `.jpg`, exactly as above. GitHub Pages is
case-sensitive, so `Jonah.JPG` will show a grey placeholder even though it
looks fine on Windows.

To nudge a face up or down in its card, edit that person's `object-position`
line in the `<style>` block — there is a comment above them explaining it.
Lower number = face sits lower.

Nothing in `index.html` needs changing. Until a file is added, that card shows
a clean grey block with the person's initials.

## Publish on GitHub Pages

1. Create a new repository on GitHub and upload everything in this folder.
2. Repo → **Settings** → **Pages**.
3. Under **Source**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Save. The site appears at `https://<username>.github.io/<repo>/` within a minute or two.

All paths are relative, so it works at any URL — root domain or subfolder.

## Editing

- Brand red and the off-white background are set once at the top of the
  `<style>` block, under `BRAND TOKENS`. Change `--brand` and it updates sitewide.
- The footer year updates itself.
