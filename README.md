# aarushiguptamemorial.org

A memorial site for Aarushi Gupta, and a quiet introduction to the family-funded
scholarship offered in her name.

## What this is

Five pages:

- `/` — landing
- `/aarushi.html` — in her glory (photo-led, the heart of the site)
- `/fund.html` — the Aarushi Gupta Memorial Fund (family-funded, awarding informally)
- `/family.html` — the people carrying her forward
- `/reach.html` — contact (contact@aarushiguptamemorial.org)

The site is built to **give, not take**. There is no donate flow.

## Visual register

Warm cream background, color photographs, one vibrant accent, soft serif body
(Lora), elegant serif display (Cormorant Garamond), generous white space. The
site is meant to burst with life.

## Build

    npm install
    npm run build         # writes ./dist
    npm run dev           # watches CSS

## Deploy (later)

GitHub Pages from `Zetetic-Dhruv/aarushiguptamemorial.org`, custom domain at
the apex. Google Workspace MX records preserved so `contact@` keeps working.

## Filling in real content

Every placeholder in the HTML is wrapped in `<div class="placeholder">…</div>`
or sits inside a `<div class="photo …">[photo]</div>` slot. Search for those
markers to find what's waiting on the family.
