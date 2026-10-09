# TIGC Virtual Try-On – interactive prototype

A clickable mobile prototype (360×800) of the TIGC virtual try-on flow, built from the Figma designs.
Plain HTML/CSS/JS – no build step, no dependencies.

## Run locally
```bash
python3 -m http.server 5173
# open http://localhost:5173
```
(Serve it over http – opening `index.html` directly will not allow the camera.)

## What's in it
- Full PDP (photos, price, coupons, sizes, highlights, reviews, similar products)
- First-time try-on: intro sheet → choose photo (camera / gallery) → Orbit loader → reveal → "Regenrate" sheet → Virtual Closet
- Second-time try-on on any product ("View Similar" opens other products): one tap → capsule fade → "Item Added" → loading → tick → final look → "Regenrate"

## Files
- `index.html` – the whole prototype
- `assets/` – images and icons exported from Figma

## Notes
- Fonts (Pretendard, Roboto, Gloock, Inter) load from CDNs, so an internet connection is needed.
- The try-on result is a fixed sample image; uploaded photos stay in the browser.
