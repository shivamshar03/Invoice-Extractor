# Invoice Extraction Bot

An intelligent application that extracts key information from invoice PDFs using AI. This tool helps automate the process of data extraction from invoices, saving time and reducing manual effort.

## Features

- Upload multiple PDF invoices simultaneously
- Extract key information including:
  - Invoice number
  - Description
  - Quantity
  - Date
  - Unit price
  - Amount
  - Total
  - Email
  - Phone number
  - Address
- Export extracted data to CSV format
- User-friendly Streamlit interface

## Prerequisites

- Python 3.x
- pip (Python package installer)

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd project-13
```

2. Create and activate a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows, use: .venv\Scripts\activate
```

3. Install the required dependencies:
```bash
pip install -r requirements.txt
```

4. Set up environment variables:
Create a `.env` file in the project root and add your API keys:
```
GROQ_API_KEY=your_groq_api_key
```

## Usage

1. Start the application:
```bash
streamlit run app.py
```

2. Open your web browser and navigate to the URL shown in the terminal (typically http://localhost:8501)

3. Upload one or more PDF invoices using the file uploader

4. Click the "Extract Data" button to process the invoices

5. View the extracted data in the interface

6. Download the extracted data as a CSV file using the download button

## Technical Details

The application uses:
- Streamlit for the web interface
- LangChain and Groq for AI-powered text extraction
- PyPDF for PDF processing
- Pandas for data manipulation

## Project Structure

```
project-13/
├── app.py              # Main Streamlit application
├── utils.py            # Utility functions for PDF processing and data extraction
├── requirements.txt    # Project dependencies
└── .env               # Environment variables (create this file)
```

## Contributing

Feel free to submit issues and enhancement requests!
