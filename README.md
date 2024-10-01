# ChatPDF-A-chatbot-for-talking-with-your-PDF

# Document Reading App like ChatGPT

This application is built using **Streamlit** to enable users to upload PDF, DOCX, or TXT files, extract text from them, and ask questions about the document's content using **OpenAI's GPT-3**.

## Features

- **File Upload**: Supports uploading `.pdf`, `.docx`, and `.txt` files.
- **Text Extraction**: Automatically extracts text from uploaded files based on file type.
- **AI-Powered Q&A**: Utilizes GPT-3 to generate questions and answers based on the extracted document text.
- **Clipboard Copy**: Provides an option to copy the generated answers directly to the clipboard.

## Setup Instructions

### 1. Clone the Repository
```bash
git clone <repository_url>
cd <repository_folder>
```

### 2. Install Dependencies
Make sure you have Python installed (preferably version 3.8 or higher). Install the required dependencies using:
```bash
pip install -r requirements.txt
```

**Required Libraries:**
- `streamlit`
- `PyPDF2`
- `openai`
- `docx2txt`
- `pyperclip`
- `io`

### 3. Set Up OpenAI API Key
Before running the app, you will need an **OpenAI API key** to use GPT-3 for text generation.
1. Obtain your OpenAI API key from [OpenAI](https://beta.openai.com/signup/).
2. Enter the API key in the app's sidebar.

### 4. Run the App
Once everything is set up, run the Streamlit app using the following command:
```bash
streamlit run app.py
```

### 5. Upload a Document
- You can upload `.pdf`, `.docx`, or `.txt` files.
- The app will extract the text and allow you to ask questions based on the document content.

### 6. Generate Answers
- The app will use GPT-3 to generate a question based on the uploaded document.
- You can also input your own question, and the app will generate a response using GPT-3.

### 7. Copy to Clipboard
- After generating an answer, you can click the "Copy Answer" button to copy the text to your clipboard.

## Usage

1. **Upload a File**: Select a `.pdf`, `.docx`, or `.txt` file using the file uploader.
2. **Automatic Question**: The app will generate a question based on the document text.
3. **Ask a Question**: You can type in a question about the document.
4. **Get an Answer**: GPT-3 will generate an answer to the question, which can then be copied to your clipboard.

## Error Handling
- If the file format is unsupported, the app will display an error message.
- Ensure that the file type is either PDF, DOCX, or TXT for successful processing.

## Customization

- To change the GPT-3 engine or adjust the prompt length, you can modify the `generate_questions()` and `generate_answers()` functions in the code.
- Adjust the maximum token limits, temperature, or other GPT-3 parameters to suit your needs.

---

