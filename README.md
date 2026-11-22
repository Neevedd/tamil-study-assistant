# Tamil Study Assistant

A Tamil-first, voice-friendly study assistant. Upload a scanned textbook page or PDF, ask questions in Tamil, Tanglish or English, and get answers from your own material, with page references, spoken aloud.

> Status: work in progress (started November 2026)

## Why this project
Study material in Tamil is often scanned, and Tamil OCR is unreliable. Visually impaired students depend on others to read and write for them. This project aims to make studying from Tamil material more independent.

## Planned features
- [ ] Reliable Tamil OCR: several engines cross-checked, with "unclear word" warnings
- [ ] Question answering from the uploaded document only, with page references
- [ ] Questions in Tamil script, Tanglish, or English
- [ ] Spoken answers in Tamil
- [ ] Voice questions
- [ ] Keyboard, screen-reader, large-font and high-contrast support

## How it works
1. Upload a PDF or photo of a page
2. OCR extracts the text
3. Text is split into chunks and embedded
4. A question retrieves the best passages
5. An LLM answers using only those passages
6. The answer is spoken aloud

(Architecture diagram to be added.)

## Tech stack
Python, FastAPI, vector database, OCR engines, open-source Tamil text-to-speech, Docker, Hugging Face Spaces (planned).

## Getting started
```bash
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt
```
(Run instructions to be added.)

## Results
Benchmarks to be added: OCR accuracy per engine, retrieval accuracy for Tamil / Tanglish / English questions.

## Accessibility
To be documented, together with feedback from real student testing.

## Privacy
Uploaded documents are meant to be deleted after the session. To be confirmed and documented.

## Roadmap
- [ ] Phase 1: Setup
- [ ] Phase 2: OCR
- [ ] Phase 3: Question answering + early deploy
- [ ] Phase 4: Tamil and Tanglish input
- [ ] Phase 5: Voice
- [ ] Phase 6: Interface and accessibility
- [ ] Phase 7: Quality (tests, CI, logging)
- [ ] Phase 8: Deployment
- [ ] Phase 9: Showcase (user testing, write-up, demo video)

## Author
Nivedhini Pari
