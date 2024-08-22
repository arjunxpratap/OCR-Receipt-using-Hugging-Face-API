OCR Receipt Using Hugging Face API
Project Overview
This project demonstrates the use of Optical Character Recognition (OCR) to extract text from receipt images using Hugging Face's TrOCR model. Additionally, it integrates OpenAI's GPT API to enhance the text processing, allowing for the extraction of structured data such as receipt numbers, dates, and total amounts. This project showcases the application of modern AI and NLP tools in real-world document processing tasks.

Features
OCR with Hugging Face's TrOCR Model: Leverages a transformer-based model to extract text from images of receipts.
Text Refinement with GPT: Uses OpenAI's GPT API to refine and correct the OCR output, ensuring accurate extraction of critical data.
Field Extraction: Automatically extracts essential fields such as receipt numbers, dates, and total amounts from the processed text.
Entity Recognition: Optionally applies NLP techniques to identify and categorize different entities within the text.
Getting Started
Prerequisites
Ensure you have the following libraries installed:

bash
Copy code
pip install transformers torch pillow openai opencv-python
Installation
Clone the Repository:

bash
Copy code
git clone https://github.com/arjunxpratap/OCR-Receipt-using-Hugging-Face-API.git
cd OCR-Receipt-using-Hugging-Face-API
Set Up API Keys:

Hugging Face: Configure your Hugging Face API token if needed.
OpenAI: Set up your OpenAI API key for GPT processing.
Run the Project:

Open the provided Jupyter notebook in Google Colab or locally.
Upload your receipt image and execute the notebook cells.
Usage
Extracted Text: The project extracts raw text from receipt images.
GPT Processing: The extracted text is passed through GPT for refinement, correcting OCR errors, and presenting the data more clearly.
Field Extraction: Key fields (e.g., Receipt Number, Date, Total Amount) are extracted from the GPT-processed text.
Entity Recognition (Optional): Further analyze the text to identify and categorize entities.
Example Output
Raw OCR Text:
mathematica
Copy code
Extracted Text: Receipt #67890 Date: 2024-08-22 Total: $45.67
Processed GPT Text:
yaml
Copy code
Receipt Number: 67890
Date: 2024-08-22
Total Amount: $45.67
Extracted Fields:
python
Copy code
{
    "Receipt Number": "67890",
    "Date": "2024-08-22",
    "Total Amount": "$45.67"
}
License
This project is licensed under the MIT License - see the LICENSE file for details.

Contributing
Contributions are welcome! Please feel free to submit a Pull Request or open an Issue to improve this project.
