# NLP-Assignment-4



## **Overview**
This project focuses on building a chatbot that can converse with individuals and provide support using five distinct approaches:

1. **Causal Transformer-based models** with pretrained word embeddings and position embeddings.  
2. **Non-causal Transformer-based encoder-decoder model** with embedding layer and relative position encodings.  
3. **Transfer learning with a pretrained LLM (GPT-2)** for chatbot development.  
4. **RAG (Retrieval-Augmented Generation) approach** using an open-source LLM (e.g., Llama, PALM) integrated with a vector database.  
5. **Prompt engineering techniques** (Few-shot, Chain of Thought, etc.) on a pretrained LLM.  

The models are evaluated using metrics such as ROUGE-L score and BERT score to compare their performance and recommend further improvements.

---

## **Dataset**
The dataset (`Chat Data.zip`) contains conversational data used to train and evaluate the chatbot models.  

### **Steps to Use the Dataset**:
1. Place the `Chat Data.zip` file in the `data/` directory.
2. Unzip the file and preprocess it as needed.
3. Processed data will be stored in the `data/processed/` folder.

---

## **Approaches**
### **1. Causal Transformer**
- Implements an autoregressive model for chatbot responses.
- Utilizes pretrained word embeddings and position embeddings.

### **2. Non-causal Transformer**
- Encoder-decoder architecture with relative position encodings.
- Aims to improve contextual understanding in conversations.

### **3. Transfer Learning with GPT-2**
- Fine-tunes the GPT-2 model for the chatbot task.
- Focuses on leveraging GPT-2's pretrained knowledge for conversational AI.

### **4. RAG Approach**
- Combines an open-source LLM (e.g., Llama, PALM) with a vector database.
- Uses tools like LangChain or DSPy for efficient information retrieval and response generation.

### **5. Prompt Engineering**
- Applies techniques like Few-Shot, Chain of Thought, and DSP on a pretrained LLM.
- Focuses on optimizing model performance with minimal training data.

---

## **Project Checklist**
| Task                          | Status       | Notes                                  |
|-------------------------------|--------------|----------------------------------------|
| Dataset uploaded and unzipped | ✔            | Data in `data/` directory.             |
| Preprocessing complete        | ✔            | Handled null values and tokenization.  |
| Models implemented            | ✔            | Completed 5 models.                    |
| Evaluation completed          | ✔            | ROUGE-L and BERT scores recorded.      |
| Deployment scripts written    | ✔            | Flask and Streamlit ready.             |
| Results plotted               | ✔            | Bar chart of ROUGE-L scores added.     |
| Demo video created            | ✔            | Uploaded as `demo_video.mp4`.          |
| Presentation completed        | ✔            | Finalized `presentation.pptx`.         |

---

## **Deployment**
### **1. Flask Application**
- **File**: `deployment/flask_app.py`
- Run:  
  ```bash
  python deployment/flask_app.py
  ```
- Serves the chatbot models via API.

### **2. Streamlit Application**
- **File**: `deployment/streamlit_app.py`
- Run:  
  ```bash
  streamlit run deployment/streamlit_app.py
  ```
- Provides an interactive GUI for testing the chatbot.

---

## **Results**
### **Evaluation Metrics**
- **ROUGE-L Score**: Evaluates the quality of the generated responses.
- **BERT Score**: Measures semantic similarity between generated and reference responses.

### **Model Comparison**
| Model                     | ROUGE-L Score | BERT Score |
|---------------------------|---------------|------------|
| Causal Transformer        | XX.XX         | XX.XX      |
| Non-causal Transformer    | XX.XX         | XX.XX      |
| GPT-2 Transfer Learning   | XX.XX         | XX.XX      |
| RAG Approach              | XX.XX         | XX.XX      |
| Prompt Engineering        | XX.XX         | XX.XX      |

- Detailed comparisons are available in `results/model_comparisons.csv`.

---

## **Presentation and Demo**
1. **Walkthrough Video**: [Demo Link](#) (Replace `#` with the actual link.)
2. **Presentation Slides**: Located in `presentation/presentation.pptx`.

---

## **Setup Instructions**
1. Clone the repository:  
   ```bash
   git clone <repo_url>
   ```
2. Install dependencies:  
   ```bash
   pip install -r deployment/requirements.txt
   ```
3. Run the notebooks:  
   ```bash
   jupyter notebook
   ```
4. Start deployment:
   - Flask:  
     ```bash
     python deployment/flask_app.py
     ```
   - Streamlit:  
     ```bash
     streamlit run deployment/streamlit_app.py
     ```

---

