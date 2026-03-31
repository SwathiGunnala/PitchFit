# PitchFit

**PitchFit** is a product concept for generating **ATS-friendly resumes** tailored to a **specific job description (JD)**—so candidates spend less time reformatting and more time on substance and stories.

**Author:** [Swathi Gunnala](https://github.com/SwathiGunnala)

## Status

This repository is in **early setup**. The README documents intent and guardrails; application code will land here as the MVP is built.

## Problem

Applicants often submit a **generic resume** to many roles. ATS systems and recruiters reward **keyword and scope alignment** with the posting. Doing that manually for every application is slow and error-prone.

## Product direction (draft)

- **Input:** Base resume + target JD (paste or upload).  
- **Output:** A structured resume variant that preserves truth while improving **fit**, **readability**, and **ATS parsing** (headings, bullets, section order).  
- **Principles:** User reviews every material change; no fabricated employment or credentials.

## Privacy & safety (non-negotiable)

- Treat pasted **JD and resume text** as sensitive; design for **minimal retention** and clear **delete** behavior.  
- Prefer **client-side or ephemeral processing** where possible; document what leaves the device.  
- Avoid storing raw documents in public logs or analytics.

## Planned stack (TBD)

Likely a small web app (e.g. React/Next or similar) with explicit sections for inputs, diff/preview, and export (PDF/Markdown). Final choices will be reflected in `package.json` when code exists.

## Repository layout

| Path | Purpose |
|------|---------|
| `README.md` | Product intent and status (this file) |
| `.gitignore` | Ignore rules once Node/build artifacts exist |

## License

[MIT License](./LICENSE)

---

**Want to contribute later?** Open an issue describing the workflow you want (e.g. “paste JD only” vs. “upload PDF”). For job-search use today, pair this repo with your live tools and keep this README updated as PitchFit ships.
