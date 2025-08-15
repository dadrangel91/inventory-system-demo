# Inventory System Demo (Barcode Scanner + CSV Log)

A zero-cost, mobile-friendly **inventory & shipping/receiving mock** you can demo from any phone or laptop. 
It scans barcodes with the camera, logs transactions (IN/OUT), and lets you **export a CSV** for sharing or analysis.

> Built for a quick proof-of-concept demo at work (Chart Industries) with no backend required.

---

## Features
- **Camera barcode scanner** (ZXing in the browser)
- **Single-page app** (just open `index.html`)
- **Transaction log** with item, quantity, action (IN/OUT), and timestamp
- **CSV export** (`transactions-YYYY-MM-DD.csv`)
- **Mobile-friendly UI** for warehouse floor use

## Quick Start
1. Download this repo (or the single-file starter) and open `index.html` in **Chrome** or **Edge**.
2. Allow **camera** access when prompted.
3. Point at a barcode → the code appears in the input field.
4. Choose **IN** or **OUT**, enter **Qty**, and click **Add**.
5. When done, click **Export CSV** to download your log.

> If iOS blocks camera access when opening a local file, serve it with a local web server or host on GitHub Pages (see below).

## GitHub Pages (optional)
1. Commit your files to the `main` branch.
2. In your repo: **Settings → Pages → Deploy from a branch → Branch: `main` / `/ (root)` → Save**.
3. Your demo will be live at `https://<your-username>.github.io/<your-repo>/`.

## File Overview
- `index.html` – Single-page scanner + logger (drop-in demo)
- `README.md` – This file
- `LICENSE` – MIT
- `.gitignore` – (empty for now)

## Roadmap (nice-to-have)
- CSV **import** to preload catalog
- **User roles** and PIN pad
- **SKU → description lookup** from a JSON/CSV
- **Offline storage** (IndexedDB) so logs persist after refresh
- **Signature/photo** capture for shipments
- **REST API** or Google Sheets connector (for real data sync)

---

## License
MIT — free to use internally or as a starting point for a production pilot.
