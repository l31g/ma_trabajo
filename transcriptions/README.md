# Transcriptions and extraction notes

This folder keeps durable extraction findings inside the repo so they are not lost in temporary session folders.

## Handling rules

- Treat all source PDFs and screenshots as sensitive.
- Do not paste raw employee IDs, addresses, dependent details, account numbers, or full benefits-cost tables into notes unless needed.
- Prefer redacted summaries and short excerpts tied to a source file.
- Keep full source documents in their original folders.

## Current extraction status

- PDF text extraction was run locally with Python/PyMuPDF.
- OneDrive PDF and Office-file text extraction was run locally from `onedrive_docs/`.
- Downscaled image copies were created locally for review/OCR.
- Local OCR was started with RapidOCR for screenshots; only partial screenshot OCR completed before interruption.
- Screenshot review after the OneDrive export used compressed, lower-resolution copies created in the session workspace. Source screenshots in the repo were not modified.
- Cloud/vision review was used only on compressed transition-resource screenshots after approval. It was **not** used for sensitive personal benefits/enrollment records.
- If cloud/vision review is used later, use compressed/downscaled images and avoid documents with personal identifiers unless explicitly necessary.

## Files

- `transition-emails-and-packet.md` - extracted findings from transition emails and the RCM resource packet.
- `benefits-enrollment-summary.md` - redacted findings from 2024-2026 JHU benefit confirmations.
- `screenshot-ocr-partial.md` - partial local OCR/findings from the HR FAQ screenshots and OneDrive screenshot-only documents.
- `personalized-letter-redacted.md` - redacted transcription of the personalized transition letter.
- `document-coverage-index.md` - source-by-source coverage index for transcripts, redacted summaries, and screenshot summaries.
- `extracted/` - full text transcripts for policy, general transition documents, and user-approved sensitive benefits confirmations.
