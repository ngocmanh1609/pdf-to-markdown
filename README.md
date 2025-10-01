# Convert PDFs to Markdown with Local LLMs

Fast, private, and free PDF-to-Markdown conversion using a local LLM (e.g., Gemma 3 via Ollama). No cloud APIs, no tokens, no privacy concerns — just elegant Python.

**Resource**: [Convert PDFs to Markdown using Local LLMs — Fast, Private, and Free](https://medium.com/data-science-collective/convert-pdfs-to-markdown-using-local-llms-c5232f3b50fc?sk=9b0036a7ff93a1c48bae7dd8216dc671)

## Installation (Using [poetry](https://python-poetry.org/))

```bash
poetry install
poetry shell
```
Then run:
```bash
python src/pdf_2_markdown_1.py
```

## Dependencies

- PyMuPDF (for PDF rendering) — not free for commercial use
- Pillow
- Ollama
- A local model like gemma3:12b or gemma3:4b must be installed and pulled

## Alternative: Fully Open Source Version

Use `pdf2image` + `Poppler` instead of `pymupdf`.

```bash
brew install poppler  # or sudo apt install poppler-utils
```
Then run:
```bash
python src/pdf_2_markdown_2.py
```

## Features

- Handles scanned PDFs via image input
- Converts to clean, structured Markdown
- Works offline with local models
