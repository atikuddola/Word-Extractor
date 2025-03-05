# PDF Word Extractor

A Python tool that extracts words from PDF documents and generates formatted PDF word lists. Supports both unique word extraction and full text parsing.

## Features
- Extract words with case sensitivity options
- Preserve original word sequence
- Handle hyphenated words and contractions
- Generate formatted PDF output with two-column layout

## Installation
```bash
pip install -r requirements.txt
```

**Dependencies**:
- PyPDF2 (PDF text extraction)
- reportlab (PDF generation)
- regex (advanced word matching)

## Usage
```bash
python extractor.py input.pdf output.pdf [--unique] [--case-sensitive]
```

**Options**:
- `--unique`: Only extract unique words
- `--case-sensitive`: Preserve original capitalization

## Example
```bash
# Extract all words preserving case
python extractor.py document.pdf wordlist.pdf --case-sensitive

# Extract unique words only
python extractor.py document.pdf unique_words.pdf --unique
```

## Output Includes
- Numbered word list
- Total word count
- Page-order preservation
- Clean formatting for printing/study
