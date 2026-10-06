# TenderFlow — Unique Tender Package Builder

A redesigned version of the supplied Tender Package Builder problem.

## Included
- Modern responsive dashboard UI
- Tender requirements JSON loader
- PDF drag & drop / multi-upload
- SHA-256 duplicate detection
- PDF page counting and validation
- One-to-one requirement ↔ PDF matching
- Mandatory / optional document states
- Expiry validation against submission deadline
- Search and status filters
- English / Bangla UI switch
- Final combined PDF generation
- Cover page + ordered documents + page footer
- 30 PDF / 50 MB browser-side limits
- No backend; files remain in the browser

## Run
```bash
npm install
npm run dev
```

Then open the Vite local URL.

## Build
```bash
npm run build
npm run preview
```

## JSON format
Use the format from the original problem statement:
```json
{
  "tender": {
    "tender_id": "T-2026-0417",
    "title": "Supply of IT Equipment",
    "procuring_entity": "Example Directorate",
    "bidder": "Example Company Ltd.",
    "submission_deadline": "2026-10-20"
  },
  "requirements": [
    {
      "id": "R01",
      "order": 1,
      "title_en": "Trade License",
      "title_bn": "ট্রেড লাইসেন্স",
      "mandatory": true,
      "has_expiry": true
    }
  ]
}
```
