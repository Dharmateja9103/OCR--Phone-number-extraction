# OCR--Phone-number-extraction
Python scripts to extract Indian mobile numbers from screenshots using OCR and compare them with Excel records for validation.
# OCR-based Phone Number Extraction & Validation

This repository contains two Python scripts built using Google Colab to
Extract mobile phone numbers from screenshots (e.g., WhatsApp images)
using OCR, normalize them, and optionally compare them against an Excel
sheet to identify missing entries.

The scripts were written to automate a manual verification task where
phone numbers were scattered across images and spreadsheets.

## What’s inside

### 1. Baseline OCR + Excel Comparison
- Extracts phone numbers from screenshots using Tesseract OCR
- Normalizes different formats (+91, spaces, hyphens)
- Compares extracted numbers with an Excel file
- Outputs numbers present in images but missing from Excel

### 2. Improved OCR with Image Preprocessing
- Adds grayscale conversion, noise filtering, and contrast enhancement
- Uses a more permissive regex to handle OCR inconsistencies
- Extracts unique 10-digit mobile numbers
- Exports results directly to an Excel file

## Tech Stack
- Python
- Tesseract OCR (pytesseract)
- Pandas
- Pillow
- Google Colab

## Use Cases
- Data cleaning and validation
- Automating manual record checks
- Extracting structured data from screenshots
- Ops/admin / research preprocessing workflows

## Notes
These scripts were developed iteratively by tuning OCR preprocessing
steps based on real screenshot quality, rather than relying on a fixed
format.

