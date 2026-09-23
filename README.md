# WSC Meet Documents

This repo is the **final publishing step** for meet documents that need to go
on **windsorswimmingclub.co.uk** — promoter's conditions, entry forms,
timetables, results packs, and similar.

**Why this exists:** WordPress's Media Library is fiddly to upload into and
everything lands in one disorganized, date-based bucket. This repo replaces
that step for meet documents. Instead of uploading into WordPress, you drop
the *finished* file here, GitHub hosts it, and you paste the resulting link
straight into the news post.

## How this fits with Google Drive

Drafting, versions-in-progress, and general storage for these documents stay
exactly where they are today — in Google Drive. Nothing about that changes.

This repo is **only** for the finished version of a document, at the moment
it's ready to go live on the website:

1. Finish/approve the document in Drive as normal.
2. Download the final file from Drive.
3. Upload that one file here, into the right season folder (see below).
4. Grab its link and paste it into the WordPress post.

If a document gets revised after publishing, re-upload the updated file here
under the same name (or a new one) — GitHub keeps the old versions in its
history either way, so nothing is lost by overwriting.

**Do not put anything sensitive here.** This repo is public (that's what
makes the links work), so only put files that are meant to be public anyway
— the same kind of document you'd currently upload to the website. Never put
entry lists, swimmer personal details, medical info, or anything with
children's personal data in here.

## Adding a document (no git required)

1. Go to the `meets` folder above, then open (or create) the season folder,
   e.g. `2026-27`.
2. Click **Add file → Upload files** (top right of the file listing).
3. Drag your PDF/Excel/Word file in, then scroll down and click
   **Commit changes**.
4. That's it — the file is now live within about a minute.

To create a new season folder, or a subfolder for a specific meet, use
**Add file → Upload files** and type the folder path into the file name box
before the file name, e.g. `2027-28/spring-open/entry-form.pdf` — GitHub
creates the folder automatically.

### Naming files

Keep names descriptive and avoid spaces where possible (use hyphens) so the
links stay clean, e.g.:

```
meets/2026-27/L3-Autumn-Sparkler-Promoter-Conditions.pdf
meets/2026-27/L3-Autumn-Sparkler-Summary-Entry-Form.xlsx
```

## Getting the link to paste into WordPress

Every file gets a permanent public link in this pattern:

```
https://windsorsc-admin.github.io/WSC-Meet-Documents/<path-to-file>
```

So a file uploaded to `meets/2026-27/entry-form.pdf` is live at:

```
https://windsorsc-admin.github.io/WSC-Meet-Documents/meets/2026-27/entry-form.pdf
```

You can work out the link yourself from the path, or: open the file in
GitHub, click the **⋯ (or "Raw")** menu — the file's path shown in the
breadcrumbs at the top of the page is exactly what goes after
`.github.io/meet-documents/`.

Paste that link as the "Promoter's Conditions" / "Entry Form" link in your
WordPress news post, exactly as you do today — the only thing that's changed
is where the file itself lives.

## One-time setup (only needs doing once, by Matt)

This repo needs **GitHub Pages** turned on before links will work:

1. On GitHub, go to this repo's **Settings → Pages**.
2. Under "Build and deployment", set **Source** to **Deploy from a branch**.
3. Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
4. Wait a minute or two for the first deploy — GitHub will show the live
   URL at the top of that same Pages settings page once it's ready. Confirm
   it matches `https://windsorsc-admin.github.io/WSC-Meet-Documents/`.

After that, every future push publishes automatically — nothing else to
configure.

## Optional: a friendlier web address later

If you'd rather these links read `files.windsorswimmingclub.co.uk/...`
instead of the `github.io` address, that's a one-time DNS change (a CNAME
record) wherever the club's domain is managed — worth doing later if these
links end up being shared a lot, not needed to get started.
