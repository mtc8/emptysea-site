# emptysea.app

The EmptySea company site, served by GitHub Pages at <https://emptysea.app>.

| Path | What it is |
|---|---|
| `index.html` | Company home — what EmptySea is, the apps, support |
| `privacy.html` | Craps Lab privacy policy |
| `craps-lab/` | The Craps Lab field guide |
| `site.css` | Shared palette and layout, taken from the field guide |
| `CNAME` | Tells GitHub Pages to serve this at emptysea.app |

The palette is the Craps Lab felt and gold, so the company site and the product
guide read as one thing.

**Note:** the older guide-only site at `mtc8/craps-lab-guide` is still live and
still the URL on the Google Play listing. Leave it alone until Play production
review finishes; the listing gets pointed here afterwards.


---

## Changing the words yourself

You don't need any tools. Do it in a browser, from any machine.

1. Go to <https://github.com/mtc8/emptysea-site>
2. Click the file you want:
   - **`index.html`** — the home page (apps, silk, support, about)
   - **`privacy.html`** — the Craps Lab privacy policy
3. Click the **pencil icon**, top right
4. Change the words
5. Scroll down and click the green **Commit changes** button

The live site updates about a minute later. If you still see the old text,
hard-refresh with **Ctrl+F5**.

### The one rule

Change only the words. Never touch anything inside angle brackets.

    <p class="lede">The other half of the company. Curated 100% mulberry silk.</p>
                    ^^^^^^^^^ this is yours to change ^^^^^^^^^

`<p class="lede">` and `</p>` are plumbing. Deleting one breaks the layout of
everything below it on that page.

### You cannot do real damage

Every version is kept forever. If a page comes out wrong, it can be put back
exactly as it was in seconds — click **History** on the file to see every
version, or just ask Claude to revert it.

### The bits most likely to need editing

- **The silk launch date** — appears twice in `index.html`, in the Silk section:
  the pill reading *On sale late September 2026*, and the line *Not on sale yet*.
  **If the date slips, change both**, or the page is making a promise that has
  already expired.
- **A buy link for silk** — when there's a store, that section should get a real
  button instead of an email address.
- **Count Lab's status** — currently *In development*. Becomes a store link when
  it ships.
- **Craps Lab on iOS** — the page deliberately says nothing about the App Store,
  because it is not approved there. See `CrapsLab/CrapsStore/apple-submission.md`.

### What NOT to change without thinking

- **`CNAME`** — this is what points emptysea.app at the site. GitHub rewrites it
  by itself when the custom domain is touched in Settings. Leave it alone.
- **The "Nothing here is gambling" notice** on the home page. It is load-bearing
  for the app stores, not decoration.
- **The privacy policy** — it is a statement about what the app actually does.
  If it stops matching the app, it has to be corrected in the app or the policy,
  not softened here. The same text is also published at
  <https://sites.google.com/view/crapslabpp/home>, which is the URL the Google
  Play listing currently points at, so **the two must not drift apart.**
