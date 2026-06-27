# QR & Barcode Generator

Generate QR codes & barcodes instantly. Supports text, URLs, SKUs, Wi-Fi, email & phone. Customize colors, size, and embed your brand logo directly into the QR code. Choose from 8 barcode formats including CODE 128, EAN-13 & UPC-A. Download as PNG or SVG — no sign-up needed.

---

## Features

### QR Code Generator
- **Content types** — free text, URL, email, phone number, SKU/product ID, and Wi-Fi credentials (auto-formats to the correct QR standard)
- **Brand logo overlay** — upload any PNG, JPG, SVG, or WebP image as a centered logo; supports drag & drop
- **Logo controls** — adjustable logo size (10–35% of QR area) and white padding around the logo
- **Error correction** — four levels: L (7%), M (15%), Q (25%), H (30%). Use Q or H when embedding a logo
- **Color customization** — independent QR color and background color pickers
- **Size control** — output from 128px to 512px
- **Download** — export as high-resolution PNG

### Barcode Generator
- **8 formats** — CODE 128, EAN-13, UPC-A, EAN-8, CODE 39, ITF-14, MSI, Pharmacode
- **Color customization** — bar color and background color pickers
- **Layout controls** — bar width, bar height, and label font size sliders
- **Text label** — toggle the human-readable text below the barcode on or off
- **Download** — export as PNG or scalable SVG (vector)

---

## Getting Started

This is a single self-contained HTML file with no build step or server required.

1. Download `qr-barcode-generator.html`
2. Open it in any modern browser
3. Start generating — no installation, no sign-up, no internet connection needed after the page loads

---

## Usage

### Generating a QR code

1. Select the **QR Code** tab
2. Choose a content type from the dropdown (URL, text, SKU, Wi-Fi, etc.)
3. Enter your content in the text area — the preview updates live
4. Adjust colors, size, and error correction level as needed
5. Click **Download PNG** to save

### Adding a brand logo

1. Generate a QR code first (use error correction level **Q** or **H** for best results with a logo)
2. Click the logo upload area or drag and drop an image file
3. Adjust the logo size and padding sliders
4. Download — the logo is baked into the exported PNG

### Generating a barcode

1. Select the **Barcode** tab
2. Choose a format from the dropdown
3. Enter a valid value for that format (see format guide below)
4. Adjust styling as needed
5. Click **Download PNG** or **SVG**

---

## Barcode Format Guide

| Format | Use case | Value example |
|---|---|---|
| CODE 128 | General purpose, alphanumeric | `ABC-12345` |
| EAN-13 | Retail products (international) | `5901234123457` (13 digits) |
| UPC-A | Retail products (North America) | `042100005264` (12 digits) |
| EAN-8 | Small retail packaging | `12345670` (8 digits) |
| CODE 39 | Industrial, logistics | `HELLO-WORLD` |
| ITF-14 | Shipping cartons | `12345678901231` (14 digits) |
| MSI | Inventory, warehouse | `12345` |
| Pharmacode | Pharmaceutical packaging | `1234` |

---

## Tech Stack

| Library | Version | Purpose |
|---|---|---|
| [qrcode](https://github.com/soldair/node-qrcode) | 1.5.4 | QR code generation to canvas |
| [JsBarcode](https://github.com/lindell/JsBarcode) | 3.11.6 | Barcode rendering to SVG |
| Space Grotesk | — | UI typography (Google Fonts) |

No frameworks, no bundler, no backend. Pure HTML, CSS, and vanilla JavaScript.

---

## Browser Support

Works in all modern browsers — Chrome, Firefox, Safari, and Edge. No polyfills required.

---

## License

MIT — free to use, modify, and distribute.
