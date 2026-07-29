# Client Handout Library

This repository stores client/adopter handouts (like "Going Home with..." guides), organized by body system, and shows them on a simple webpage that anyone with the link can browse, download, or print from — no GitHub account needed to view it.

You do **not** need to know how to code to use this. Everything below is done by clicking around on the GitHub website.

---

## One-time setup (do this once)

1. **Create the repository on GitHub** (if you haven't already):
   - Go to github.com and click the **+** in the top right → **New repository**.
   - Name it something like `client-handouts`.
   - Choose **Public** if you want anyone to be able to view the page, or **Private** if it's for staff only (see note below).
   - Click **Create repository**.

2. **Upload these starter files:**
   - On your new repo's page, click **Add file → Upload files**.
   - Drag in `index.html`, `print.html`, `README.md`, and the whole `handouts` folder (with its category subfolders) from this package.
   - Scroll down and click **Commit changes**.

3. **Turn on GitHub Pages** (this makes the webpage live):
   - In your repository, click **Settings** (top menu).
   - In the left sidebar, click **Pages**.
   - Under "Build and deployment," set **Source** to **Deploy from a branch**.
   - Set **Branch** to `main` and folder to `/ (root)`, then click **Save**.
   - GitHub will show you a web address (something like `https://yourname.github.io/client-handouts/`) — give it a minute or two, then visit it. That's your library page.

> **Note on Private repos:** If you make the repo Private, GitHub Pages requires a paid plan to publish a private site. For a free option with restricted access, keep the repo Public but don't share the link widely — or ask about GitHub Enterprise/Organization plans if this is for internal staff only.

---

## How handouts are organized

Handouts are grouped into folders by body system, and both webpages (the library and the print tool) automatically display them grouped the same way:

```
handouts/
├── Cardiac/
├── Dermatologic/     (skin)
├── Otic/             (ear)
├── Ocular/           (eye)
├── Dental/
├── Respiratory/
├── Orthopedic/
└── Geriatric/        (senior pet care)
```

You don't have to touch any code to keep this working — just put each new handout in the folder that matches its system, and the pages pick it up automatically. If you upload a handout to a brand-new folder name that isn't one of the five above, it will still show up, just as a section labeled with the folder's name.

---

## Adding a new handout later

1. Go to your repository on GitHub.com and open the `handouts` folder.
2. Open the subfolder that matches the body system (e.g. `Otic` for an ear condition). If a handout doesn't fit any existing folder, click **Add file → Create new file**, type `NewFolderName/placeholder.txt` to make a new folder, then upload into it — or just ask Claude to tell you which folder to use.
3. Click **Add file → Upload files**.
4. Drag in the new file — upload **both** a `.docx` (editable version) **and** a `.pdf` (needed for the print tool) with the same name, e.g. `Going_Home_with_a_Broken_Bone.docx` and `Going_Home_with_a_Broken_Bone.pdf`.
5. Click **Commit changes**.

That's it — both the library page and the print page update themselves automatically within a minute or two. You don't need to touch any code.

**Naming tip:** Name files clearly, e.g. `Going_Home_with_a_Broken_Bone.docx`. The webpage turns underscores into spaces and uses the filename as the title, so a good filename = a good title on the page.

> **Why both a docx and a pdf?** The library page lets people download and edit the Word version. The print tool only works with PDFs (so it can combine several into one print job reliably) — so a PDF version needs to exist for anything you want to be selectable on the print page. If you only upload a `.docx`, you can open it in Word and use "Save As → PDF" to create the matching file, or ask Claude to generate both when it creates a new handout.

---

## Printing multiple handouts at once

1. Visit your library page and click **"Select handouts to print"** (or go directly to `.../print.html`).
2. Handouts are grouped by system, same as the library page. Check the boxes for whichever handouts you need — use "Select all in section" to grab a whole category at once.
3. Click **Print Selected**.
4. A combined PDF opens in a new tab and your browser's print dialog appears automatically — print it like any normal document.

If a print dialog doesn't appear, your browser may have blocked the pop-up — allow pop-ups for the site and click **Print Selected** again.

---

## Replacing or removing a handout

- **To replace one:** upload a new file with the *same name* in the same folder — GitHub will ask if you want to overwrite it.
- **To remove one:** open the file inside its category folder on GitHub.com, click the trash/delete icon, and commit the change.
- **To move a handout to a different system/folder:** upload it into the new folder, then delete the old copy.

---

## What's in this package

```
client-handouts/
├── index.html              <- the library webpage (don't need to edit this)
├── print.html               <- the "pick handouts and print" tool (don't need to edit this)
├── README.md                 <- this file
└── handouts/
    ├── Cardiac/
    │   ├── Going_Home_with_a_Heart_Murmur.docx
    │   └── Going_Home_with_a_Heart_Murmur.pdf
    ├── Dermatologic/
    │   ├── Going_Home_with_Allergy_Skin_Medications.docx / .pdf
    │   ├── Going_Home_with_Demodex.docx / .pdf
    │   ├── Going_Home_with_Flea_Allergy_Dermatitis.docx / .pdf
    │   └── Going_Home_with_a_Skin_Mass.docx / .pdf
    ├── Otic/
    │   ├── Going_Home_with_an_Ear_Infection.docx / .pdf
    │   └── Going_Home_with_an_Aural_Hematoma.docx / .pdf
    ├── Ocular/
    │   ├── Going_Home_After_Cherry_Eye_Surgery.docx / .pdf
    │   ├── Going_Home_After_Enucleation.docx / .pdf
    │   └── Going_Home_After_Entropion_Surgery.docx / .pdf
    ├── Dental/
    │   ├── Going_Home_with_Dental_Disease.docx / .pdf
    │   └── Going_Home_After_a_Dental_Cleaning.docx / .pdf
    ├── Respiratory/
    │   └── Going_Home_with_an_Upper_Respiratory_Infection.docx / .pdf
    ├── Orthopedic/
    │   ├── Going_Home_with_Lameness.docx / .pdf
    │   └── Going_Home_with_Patellar_Luxation.docx / .pdf
    └── Geriatric/
        └── Going_Home_with_a_Senior_Pet.docx / .pdf
```

If you'd like new handouts created in the same style as these, just ask Claude to design one (and let it know the body system) — it can hand you a matching `.docx`/`.pdf` pair ready to drop into the right folder.
