
---

# Chat PDF with Gemini 💁

This project allows users to engage in a conversational interface with PDF documents using Gemini, a conversational AI model. Users can ask questions based on the content of the uploaded PDF files, and the system will provide answers derived from the context within the documents.

## Getting Started

To get started with the project, follow these steps:

### Prerequisites

- Python 3.12.2
- Ensure you have pip installed

### Step 1: Create and Activate Virtual Environment

1. Open your command line interface (CLI).
2. Navigate to the root directory of your project.
3. Run the following commands to create and activate a virtual environment named `myenv`:

```bash
# If you're using Windows Command Prompt
python -m venv myenv
myenv\Scripts\activate

# If you're using macOS/Linux Terminal
python3 -m venv myenv
source myenv/bin/activate
```

These commands will create a virtual environment named `myenv` and activate it. You'll see `(myenv)` appear at the beginning of your command prompt, indicating that the virtual environment is active.

### Step 2: Installation

1. Clone the repository to your local machine.

```bash
git clone <repository_url>
cd <repository_name>
```

2. Install the required dependencies.

```bash
pip install -r requirements.txt
```

### Step 3: Setting up Google API Key

To utilize Google's Generative AI model, you need to obtain an API key from Google and set it as an environment variable.

1. Create a `.env` file in the root directory of the project.

2. Add your Google API key to the `.env` file.

```bash
GOOGLE_API_KEY=your_api_key_here
```

### Step 4: Running the Application

Once everything is set up, you can run the application.

```bash
streamlit run src/main.py
```

This command will start the Streamlit application, which provides a web interface for interacting with PDF files and asking questions.

## Usage

1. Upload PDF files using the file uploader interface.
2. Ask questions related to the content of the uploaded PDFs in the provided text input field.
3. Click on "Submit & Process" to initiate processing.
4. The system will extract text from the PDF files, split it into chunks, and generate embeddings for each chunk.
5. After processing, you can ask questions in the text input field, and the system will provide answers based on the context within the documents.

## Contributing

Contributions are welcome! If you'd like to contribute to the project, feel free to open an issue or submit a pull request.

---
