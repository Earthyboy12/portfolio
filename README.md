# Sethapong Lertsakulbunlue, MD — portfolio

A single static page (`index.html`) with no build step. It's deployed on Vercel, and every push to `main` redeploys it.

## Updating the CV

The Download CV buttons serve `cv/Sethapong-Lertsakulbunlue-CV.pdf`. The version and date shown next to them come from `cv.json`:

```json
{ "version": "1.1", "updated": "2026-11-15", "file": "cv/Sethapong-Lertsakulbunlue-CV.pdf" }
```

To publish a new CV:

1. Replace `cv/Sethapong-Lertsakulbunlue-CV.pdf` with the new file, keeping the same name.
2. In `cv.json`, raise `version` and set `updated` to the date in YYYY-MM-DD form.
3. Push to `main`.

The site shows the date as "15 Nov 2026" in English and "15 พ.ย. 2569" in Thai, and visitors download the file as `Sethapong-Lertsakulbunlue-CV-v1.1.pdf`.

`cv/cv.html` is the source of the current PDF. To regenerate it, edit that page (including the version and date in its header and page footer) and print it from Chrome as A4 PDF with background graphics on.
