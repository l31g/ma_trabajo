# Document transcription coverage index

This index tracks whether each document source has a full text transcript in the repo, a redacted summary, or a screenshot-only summary.

Handling rule: raw transcripts are stored for policy/general transition documents. Sensitive personal records, benefits confirmations, E210 reports, and personalized letters are represented by redacted summaries or redacted transcription notes instead of full raw text.

Update: the user approved transcribing the benefits confirmations and personalized letter. Benefits confirmations now have full text transcripts under `transcriptions/extracted/sensitive/`. The personalized letter also has an OCR transcript under `transcriptions/extracted/sensitive/`, with the employee identifier redacted.

## Full text transcripts stored in repo

| Source document | Transcript |
| --- | --- |
| `policies/HR023.pdf` | `transcriptions/extracted/policies/policies__HR023.txt` |
| `policies/HR025.pdf` | `transcriptions/extracted/policies/policies__HR025.txt` |
| `policies/HR026.pdf` | `transcriptions/extracted/policies/policies__HR026.txt` |
| `policies/HR029.pdf` | `transcriptions/extracted/policies/policies__HR029.txt` |
| `policies/HR031.pdf` | `transcriptions/extracted/policies/policies__HR031.txt` |
| `policies/JHU-JHHS-Administrative-Transfer-Guidelines.pdf` | `transcriptions/extracted/policies/policies__JHU-JHHS-Administrative-Transfer-Guidelines.txt` |
| `policies/JHHS-JHU-Administrative-Transfer-Guidelines-Frequently-Asked-Questions.pdf` | `transcriptions/extracted/policies/policies__JHHS-JHU-Administrative-Transfer-Guidelines-Frequently-Asked-Questions.txt` |
| `attachments/Revenue Cycle Transition/Resource Packet All Other Affected Staff (1).pdf` | `transcriptions/extracted/transition-docs/attachments__Revenue_Cycle_Transition__Resource_Packet_All_Other_Affected_Staff_1_.txt` |
| `onedrive_docs/RCM Transition Communications/Support Resources/Resource Packet All Other Affected Staff.pdf` | `transcriptions/extracted/transition-docs/onedrive_docs__RCM_Transition_Communications__Support_Resources__Resource_Packet_All_Other_Affected_Staff.txt` |
| `onedrive_docs/RCM Transition Communications/HR FAQs/HR FAQs.pdf` | `transcriptions/extracted/transition-docs/onedrive_docs__RCM_Transition_Communications__HR_FAQs__HR_FAQs.txt` |
| `onedrive_docs/RCM Transition Communications/HR FAQs/Q&A_ 6_5_26.xlsx` | `transcriptions/extracted/onedrive-docs/onedrive_docs__RCM_Transition_Communications__HR_FAQs__Q_A__6_5_26.txt` |
| `onedrive_docs/RCM Transition Communications/JHHS Benefits/2026 Updated Benefits Presentation 6_3_26.pdf` | `transcriptions/extracted/transition-docs/onedrive_docs__RCM_Transition_Communications__JHHS_Benefits__2026_Updated_Benefits_Presentation_6_3_26.txt` |
| `onedrive_docs/RCM Transition Communications/JHHS Benefits/Benefits-Summary_Termination.pdf` | `transcriptions/extracted/transition-docs/onedrive_docs__RCM_Transition_Communications__JHHS_Benefits__Benefits-Summary_Termination.txt` |
| `onedrive_docs/RCM Transition Communications/Open Positions_ Will Be Posted Here 6_2_26/Competitive_JobLinks_RCM Integration.docx` | `transcriptions/extracted/onedrive-docs/onedrive_docs__RCM_Transition_Communications__Open_Positions__Will_Be_Posted_Here_6_2_26__Competitive_JobLinks_RCM_Integration.txt` |
| `onedrive_docs/RCM Transition Communications/Open Positions_ Will Be Posted Here 6_2_26/Job Descriptions link.docx` | `transcriptions/extracted/onedrive-docs/onedrive_docs__RCM_Transition_Communications__Open_Positions__Will_Be_Posted_Here_6_2_26__Job_Descriptions_link.txt` |
| `onedrive_docs/RCM Transition Communications/Open Positions_ Will Be Posted Here 6_2_26/Non RCM Integration - JHHS Openings.xlsx` | `transcriptions/extracted/onedrive-docs/onedrive_docs__RCM_Transition_Communications__Open_Positions__Will_Be_Posted_Here_6_2_26__Non_RCM_Integration_-_JHHS_Openings.txt` |
| `attachments/Revenue Cycle Transition/Nieves, Wanda.pdf` | `transcriptions/extracted/sensitive/attachments__Revenue_Cycle_Transition__Nieves_Wanda.txt` |
| `benefits/2024.pdf` | `transcriptions/extracted/sensitive/benefits__2024.txt` |
| `benefits/2025.pdf` | `transcriptions/extracted/sensitive/benefits__2025.txt` |
| `benefits/2026.pdf` | `transcriptions/extracted/sensitive/benefits__2026.txt` |

Notes:

- `policies/document.pdf` is a duplicate copy of `policies/HR031.pdf`; use the HR031 transcript.
- SuccessFactors URL state tokens in extracted job-link transcripts were redacted as `[redacted]`.

## Redacted summaries or redacted transcription notes

| Source document | Coverage |
| --- | --- |
| `emails/revenue_cycle_transition.pdf` | `transcriptions/transition-emails-and-packet.md`; redacted summary. |
| `emails/lets_get_you_started.pdf` | `transcriptions/transition-emails-and-packet.md`; redacted summary. |
| `e210/FY2016.pdf` through `e210/FY2027.pdf` | `jhu-jhhs-transfer-notes.md`; redacted aggregate findings only. |

## Screenshot-only or failed-download coverage

| Source group | Coverage |
| --- | --- |
| `screenshots/HR_FAQs/` | `transcriptions/screenshot-ocr-partial.md`; later covered by downloaded `HR FAQs.pdf` transcript. |
| `screenshots/Q&A_6_5_26/` | `transcriptions/screenshot-ocr-partial.md`; superseded by downloaded `Q&A_ 6_5_26.xlsx` transcript. |
| `screenshots/Screenshot 2026-06-06 at 15.10.52.png` | `jhu-jhhs-transfer-notes.md`; policy-library screenshot summary. |
| `onedrive_docs/RCM Transition Communications/JHHS Benefits/` screenshots | `transcriptions/screenshot-ocr-partial.md`; JHHS benefits overview summary. |
| `onedrive_docs/RCM Transition Communications/PBS Teams/` screenshots | `transcriptions/screenshot-ocr-partial.md`; org-chart summary. |
| `onedrive_docs/RCM Transition Communications/Support Resources/` screenshots | `transcriptions/screenshot-ocr-partial.md`; manager packet and RIF benefits summary. |
| `onedrive_docs/RCM Transition Communications/Transition TImeline/` screenshots | `transcriptions/screenshot-ocr-partial.md`; milestones summary. |
| `onedrive_docs/___All_Errors.txt` and individual `*_Error.txt` files | `transcriptions/transition-emails-and-packet.md`; failed-download list. |

## Sources intentionally not fully transcribed into repo

- E210 annual reports remain summarized because they contain personal identifiers and detailed leave records.
- The personalized letter transcript redacts the employee identifier.
- Manager packet screenshots: marked confidential/limited distribution; summarized only.
