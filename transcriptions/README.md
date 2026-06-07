# Transcriptions and extraction notes

This folder keeps durable extraction findings inside the repo so they are not lost in temporary session folders.

## Handling rules

- Treat all source PDFs and screenshots as sensitive.
- Do not paste raw employee IDs, addresses, dependent details, account numbers, or full benefits-cost tables into notes unless needed.
- Prefer redacted summaries and short excerpts tied to a source file.
- Keep full source documents in their original folders.

## Current extraction status

- PDF text extraction was run locally with Python/PyMuPDF.
- Downscaled image copies were created locally for review/OCR.
- Local OCR was started with RapidOCR for screenshots; only partial screenshot OCR completed before interruption.
- Cloud OCR was **not** used for sensitive benefits or personal records. If cloud/vision review is used later, use downscaled images and avoid documents with personal identifiers unless explicitly necessary.

## Files

- `transition-emails-and-packet.md` - extracted findings from transition emails and the RCM resource packet.
- `benefits-enrollment-summary.md` - redacted findings from 2024-2026 JHU benefit confirmations.
- `screenshot-ocr-partial.md` - partial local OCR/findings from the HR FAQ screenshots.

