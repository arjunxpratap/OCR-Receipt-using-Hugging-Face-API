# OCR-Receipt-using-Hugging-Face-API

Project Overview
This project demonstrates the use of Optical Character Recognition (OCR) to extract text from invoice images using Hugging Face's TrOCR model, followed by advanced text processing with OpenAI's GPT API. The project is designed to extract structured data such as invoice numbers, dates, and total amounts from the raw OCR output, showcasing how modern NLP and AI tools can be leveraged for real-world document processing tasks.

Features
OCR with Hugging Face's TrOCR Model: Extract text from invoice images using a state-of-the-art transformer-based model.
Text Refinement with GPT: Use OpenAI's GPT API to correct, clean, and refine the extracted text.
Field Extraction: Automatically extract important fields such as invoice numbers, dates, and total amounts.
Entity Recognition: Optional step to recognize and categorize entities in the extracted text using an NLP pipeline.
Requirements
To run this project, you need the following Python libraries:

bash
Copy code
pip install transformers torch pillow openai opencv-python
Getting Started
Clone the Repository:

bash
Copy code
git clone https://github.com/your-username/invoice-ocr-using-huggingface-gpt.git
cd invoice-ocr-using-huggingface-gpt
Set Up API Keys:

Hugging Face: Set up your Hugging Face API token (if needed).
OpenAI: Set up your OpenAI API key to use GPT.
Run the Project:

Open the provided Jupyter notebook in Google Colab or locally.
Upload your invoice image and execute the notebook cells.
Usage
Extracted Text: The notebook will extract text from the invoice image.
GPT Processing: The extracted text is passed through GPT to refine and correct any OCR errors.
Field Extraction: The key fields (e.g., Invoice Number, Date, Total Amount) are extracted from the refined text.
Entity Recognition (Optional): Apply an entity recognition model to categorize different parts of the text.
Example Output
Raw OCR Text:
mathematica
Copy code
Extracted Text: Invoice #12345 Date: 2024-08-22 Total: $1,234.56
Processed GPT Text:
yaml
Copy code
Invoice Number: 12345
Date: 2024-08-22
Total Amount: $1,234.56
Extracted Fields:
python
Copy code
{
    "Invoice Number": "12345",
    "Date": "2024-08-22",
    "Total Amount": "$1,234.56"
}
License
This project is licensed under the MIT License - see the LICENSE file for details.

Contributing
Contributions are welcome! Please feel free to submit a Pull Request or open an Issue to contribute to this project.

