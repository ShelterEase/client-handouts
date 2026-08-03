# Updating to Resource Library

This turns your existing `client-handouts` site into a hub with 6 sections: Client Handouts, Forms, Drug Sheets, Charts, SOPs, and Templates. It's designed so you **do not need to re-upload your existing handouts** — only a few small changes to your live repo.

Do these steps in order.

---

## Step 1 \u2014 Rename your current index.html

Your current `index.html` (the client handout library) needs to become `handouts-library.html`, so the new `index.html` can become the hub page.

1. On GitHub.com, open your repo and click on `index.html`.
2. Click the pencil (Edit) icon.
3. At the top, click the filename `index.html` and change it to `handouts-library.html`.
4. Scroll down and commit directly to `main`.

Your handouts and print tool are untouched by this \u2014 only the filename changed.

---

## Step 2 \u2014 Upload the new files

Upload these files/folders from this package to the **root** of your repo (same level as `handouts/` and `print.html`):

- `index.html` (the new hub page \u2014 since you renamed the old one in Step 1, there's no naming conflict)
- `forms.html`
- `drug-sheets.html`
- `charts.html`
- `sops.html`
- `templates.html`
- `forms/` folder (contains a placeholder file)
- `drug-sheets/` folder (contains a placeholder file)
- `charts/` folder (contains a placeholder file)
- `sops/` folder (contains a placeholder file)
- `templates/` folder (contains a placeholder file)

**Easiest way:** Go to `https://github.com/ShelterEase/client-handouts/upload/main` (uploads straight to the repo root) and drag in the 5 HTML files plus the 4 folders together in one go. Since the 4 folders each only contain one small placeholder file, dragging the whole folder in at once should work \u2014 but if you hit the same "files land loose instead of in folder" issue as before, fall back to the folder-first method (create `forms/placeholder.md` as a new file to make the folder, then upload into it) for any that don't land correctly.

---

## Step 3 \u2014 Update `print.html` and old `handouts-library.html`

These two files already have updated navigation links built in (pointing back to the new hub) \u2014 just upload the versions from this package **on top of** the existing ones:

1. Go to `handouts-library.html` in your repo \u2014 click it, click the pencil to edit, delete all content, paste in the new version from this package, commit.
2. Do the same for `print.html`.

(This just adds a "\u2190 Resource Library" link to the top of each page \u2014 everything else is identical to what you have now.)

---

## Step 4 \u2014 Verify

Visit your Pages URL. You should see the new **Resource Library** hub with 6 cards. Click "Client Handouts" \u2014 it should take you to your existing library exactly as before.

---

## Adding files to a new section (Forms, Drug Sheets, Charts, SOPs, Templates)

Same pattern as your handouts:

1. Decide if you want subfolders within a section (e.g. `forms/Intake/`, `forms/Adoption/`) or just a flat list of files directly in `forms/`. Both work \u2014 subfolders show up as labeled groups on the page, and loose files show up under "All Files."
2. To upload directly into a section folder, use a URL like:
   `https://github.com/ShelterEase/client-handouts/upload/main/forms`
   (swap `forms` for `drug-sheets`, `charts`, or `templates`)
3. If you want a subfolder inside a section and it doesn't exist yet, create it first the same way you did for Orthopedic: **Add file \u2192 Create new file**, type e.g. `forms/Intake/placeholder.md`, commit \u2014 then upload into that folder.
4. Delete each `placeholder.md` once real files are in that folder (optional \u2014 it's harmless to leave, it's just filtered out of the page automatically).

---

## What's in this package

```
index.html              <- new hub page ("Resource Library")
handouts-library.html    <- your existing client handout library (renamed, nav link added)
print.html                <- your existing print tool (nav link added)
forms.html                  <- new Forms section page
forms/placeholder.md
drug-sheets.html              <- new Drug Sheets section page
drug-sheets/placeholder.md
charts.html                      <- new Charts section page
charts/placeholder.md
sops.html                              <- new SOPs section page
sops/placeholder.md
templates.html                      <- new Templates section page
templates/placeholder.md
handouts/                              <- your existing handouts, included for reference only \u2014 you already have this live, no need to re-upload
```
