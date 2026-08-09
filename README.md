# Bonnie Studio — Tools

Small self-contained pages for the studio workflow. No build step, no dependencies.

| Tool | What it does |
|---|---|
| [**intake.html**](https://chrp-bass.github.io/bonnie-studio-tools/intake.html) | New-trip intake. Bonnie fills it in, taps **Generate Trip Brief**, and gets a single `brief.txt` to download or copy. Links straight to the shared Drive for photos. |

`index.html` is a copy of the intake form, so the bare repo URL opens it too.

## The workflow

1. Bonnie fills in **intake.html** after a trip
2. Downloads `brief.txt` → it goes in `trips/<slug>/`
3. Drops every photo and video into the matching **Drive** folder — unsorted.
   Itinerary PDFs and docs go in the same folder; the engine reads them.
4. Jeff runs `make the <slug> trip`
5. The engine stops at the **story arc** for approval, then builds the package
6. Finals land in their own `bonnie-<slug>-finals` repo with a review page

**Shared Drive:** https://drive.google.com/drive/folders/1PB2VUYvt5gFRg-D7vxWzj2zc1fhJi7zS
