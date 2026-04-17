# YSI Water Quality Logger

This is a first-version Safari-friendly field app for logging YSI screen readings and exporting them into the user's spreadsheet structure.

## What it does
- Lets you choose a monitoring site and the correct depth row.
- Lets you take or upload a photo of the YSI screen.
- Runs OCR in the browser using Tesseract.js.
- Parses the fields used in the spreadsheet template:
  - Date
  - Time
  - Temp.
  - Cond.
  - Salinity
  - DO mg/L
  - DO%
  - pH
  - Turb
- Stores saved readings in browser local storage.
- Exports a `.xlsx` file using the same row structure as the uploaded template.

## Notes
- Personnel, weather, and rain remain blank for manual entry.
- Barometric pressure is intentionally ignored.
- For rows where the template has a blank depth, the app labels that option as `Deep / second row`.
- If a site/depth row is saved twice, the later reading replaces the earlier one.

## Deploy on GitHub Pages
1. Create a new GitHub repository.
2. Upload `index.html`.
3. In GitHub, go to **Settings → Pages**.
4. Set source to the main branch root.
5. Open the published URL in Safari on your phone.
6. Optionally use **Add to Home Screen** on iPhone.

## Files
- `index.html` — the app
- `Data Spreadsheet Template for App.xlsx` — your original template for reference
