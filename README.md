# Pass Designer Templates

A collection of **six ready-to-use Wallet pass templates** crafted for **Pass Designer** — Apple's new official macOS app for building and previewing Apple Wallet passes. Built by [@MCUBE76268](https://github.com/MCUBE76268) — download, open, and start designing your own passes in minutes.

---

## Getting Started

### 1. Download the Templates

Click **Code → Download ZIP** at the top of this page, then unzip the folder on your Mac.

### 2. Open in Pass Designer

1. Launch **Pass Designer** on macOS 27
2. Go to **File → Open**
3. Navigate to the `Templates/` folder inside the unzipped download
4. Open any `.pkpasstemplate` file to start editing

### 3. Make It Yours

Customize colors, fields, images, and branding — Pass Designer updates the preview in real time so you see exactly how your pass will look on iPhone and Apple Watch.

---

## Requirements

- **macOS 27** or later
- **Pass Designer** (beta) — [Download from Apple Developer](https://developer.apple.com/download/all/?q=pass%20designer)

---

## What's Inside

Six `.pkpasstemplate` files covering the most common pass types:

| Template | File | Use Case |
|---|---|---|
| ✈️ Boarding Pass | `Templates/BoardingPass.pkpasstemplate` | Flight / transit passes |
| 🏷️ Coupon | `Templates/Coupon.pkpasstemplate` | Retail discounts & promos |
| 📋 Generic | `Templates/Generic.pkpasstemplate` | Appointments & check-ins |
| 🛍️ Store Card | `Templates/StoreCard.pkpasstemplate` | Loyalty & rewards cards |
| 🎟️ Event Ticket | `Templates/Event.pkpasstemplate` | Concerts, shows & events |
| 🖼️ Poster Generic | `Templates/PosterGeneric.pkpasstemplate` | Poster-style media passes |

---

## From Template to Distributable `.pkpass`

Once you've finished designing in Pass Designer, to distribute your pass:

1. Add image assets (`icon.png`, `logo.png`, `background.png`, etc.)
2. Generate a `manifest.json` with SHA-1 hashes of all bundle files
3. Sign the manifest with your **Pass Type ID certificate** from Apple Developer
4. Zip the bundle contents (not the folder) and rename to `.pkpass`

---

## Placeholder Values

Each `pass.json` ships with placeholder identifiers — replace these before signing or distributing real passes:

```json
"passTypeIdentifier": "pass.com.passdesigner.sample",
"teamIdentifier":     "ABCDE12345",
"organizationName":   "Pass Designer"
```

---

## Legacy Samples

The `Samples/` folders contain plain `.pass` JSON bundles from earlier experiments with Pass Builder and manual signing. Kept for reference, but **Pass Designer expects `.pkpasstemplate` files** from the `Templates/` folder.

---

## Contributing

Found a bug or want to add a new pass type? PRs are welcome. Open an issue first to discuss bigger changes.

---

## Useful Links

- 🎨 [Pass Designer — Official Page](https://developer.apple.com/pass-designer/)
- 🎬 [Pass Designer — WWDC Video Walkthrough](https://youtu.be/TvB-XLSIlqg)
- 📖 [Wallet Passes — Developer Documentation](https://developer.apple.com/documentation/walletpasses)
- 🛠️ [pass-builder — Apple's Open Source Tool](https://github.com/apple/pass-builder)

---

## License

MIT License

Copyright (c) 2026 MCUBE76268

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

*Made by [@MCUBE76268](https://github.com/MCUBE76268) · If you found this useful, a ⭐ on the repo would be really nice — and feel free to credit me if you use these in your project, though no pressure at all!*
