# Conversational RAG with PDF Uploads and Chat History
This project allows users to upload PDFs and interact with the content of the PDFs using a Conversational Retrieval-Augmented Generation (RAG) model. Users can upload multiple PDFs, ask questions related to the content, and maintain a chat history that can be referenced during conversations.

### Features
- Upload PDF files and process their content.
- Use a Retrieval-Augmented Generation model to answer questions about the uploaded PDFs.
- Maintain chat history for context-based responses.
- Choose between multiple models for answering questions.
  
## Requirements
Before running the application, make sure to have the following:
1. Python 3.7+ installed.
2. Streamlit and LangChain libraries.
3. Groq API Key to use the Groq model for conversational AI.

### Python Packages:
You can install the required dependencies by running:

```bash
pip install -r requirements.txt
```
Where requirements.txt contains all the necessary libraries for this project.

### Setup Instructions
1. Clone the repository to your local machine:
```bash
https://github.com/DhanushGD/Conversational-RAG-System-for-PDF-Documents-
cd Conversational-RAG-System-for-PDF-Documents-
```

2. Create a .env file in the project root directory and add the following environment variables:
    - HF_TOKEN: Your Hugging Face API token (for embedding models).
    - LANGSMITH_API_KEY: Your Langchain API key.
    - LANGCHAIN_PROJECT: Your Langchain project key.

3. Obtain a Groq API Key by signing up at Groq API and get your API key.

4. Install dependencies:
After cloning the repository, install the required dependencies by running:
```bash
pip install -r requirements.txt
```

5. Run the Streamlit app:
After setting up everything, run the following command to start the Streamlit interface:
```bash
streamlit run app.py
```
This will open the application in your web browser, where you can interact with the PDF and ask questions.

### How to Use the Application
1. Upload PDF Files
    - On the Streamlit interface, you'll see an option to upload one or more PDF files.
    - Select the files you want to upload.
    - The app will automatically extract and process the text content from the PDFs.

2. Enter Groq API Key
    - You need to enter your Groq API Key into the input field at the top.
    - This key will enable you to interact with Groq’s conversational AI models.

3. Select a Model
    - After entering the API key, you can select the conversational model you want to use (e.g., gemma2-9b-it or Llama3-8b-8192).

4. Ask Questions
    - Once the PDFs are uploaded and the model is selected, you can type in your questions about the PDF content.
    - The system will use the Retrieval-Augmented Generation approach to answer your question based on the content from the uploaded PDFs.

5. View Chat History
    - The application will store chat history and show it on the screen. This allows for context-aware responses in your conversations with the assistant.

### Example Use Case
- Upload a research paper PDF.
- Ask questions such as "What is the main conclusion of this paper?".
- Get a concise answer based on the paper’s content.
- Maintain chat history for follow-up questions like "Can you elaborate on the methodology?".

### Notes
- PDF Processing: The application uses PyPDFLoader to extract text from PDF files.
- Model Options: The app supports multiple Groq-based models, and you can choose the one that best fits your needs.
- Persistent Chat History: The chat history is session-based and stored in the app's session state.

### Screenshots
Below are some screenshots of the app’s interface, showing the input and output interaction as well as the Langsmith models used in the application.

1. App Input - PDF Upload and Question Input
This screenshot shows the app's interface where users can upload PDF files and input their questions to interact with the content.
![Screenshot 2025-04-04 000038](https://github.com/user-attachments/assets/9559d81a-2b22-4455-90b6-75eb21c6462e)

![Screenshot 2025-04-04 000134](https://github.com/user-attachments/assets/821829c9-8e13-4c9c-84be-a087d2b0f91f)

3. App Output - Answer Based on PDF Content
This screenshot shows the app’s response after a user asks a question, based on the context extracted from the uploaded PDF.
![Screenshot 2025-04-04 000212](https://github.com/user-attachments/assets/2b00a0e0-c866-48c3-a1ba-ad2e8a6c1611)

![Screenshot 2025-04-04 000226](https://github.com/user-attachments/assets/635cff31-dfb1-45cc-988a-bd0a72b6d26f)

4. Langsmith Model Screenshot
Below is the Langsmith model interface used to select between models like gemma2-9b-it or Llama3-8b-8192.
![Screenshot 2025-04-03 235602](https://github.com/user-attachments/assets/2fb12bc1-3106-4109-a0f0-3655483e6f48)

![Screenshot 2025-04-03 235640](https://github.com/user-attachments/assets/c2334fd5-0bce-4667-bcc0-a7a88525708d)



