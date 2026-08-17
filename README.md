# 🤖 Generative AI Laboratory Experiments

A collection of **8 practical experiments** demonstrating the implementation of Generative AI concepts using **Pre-trained Foundation Models, Large Language Models (LLMs), Transformers, RAG, Code LLMs, and Diffusion Models**.

---

## 📌 Overview

This repository contains practical implementations of modern Generative AI techniques using Python and Hugging Face Transformers.

The experiments demonstrate:

* 📝 Text Generation
* 🎯 Prompt Engineering
* 💬 Conversational AI
* 📄 Text Summarization
* ❓ Question Answering
* 😊 Sentiment Analysis
* 🔎 Zero-Shot Document Classification
* 📚 Retrieval-Augmented Generation (RAG)
* 💻 AI Code Generation and Debugging
* 🎨 Image Generation using Diffusion Models

---

## 🛠️ Technologies Used

* **Python 3.9+**
* **PyTorch**
* **Hugging Face Transformers**
* **Sentence Transformers**
* **FAISS**
* **Diffusers**
* **NumPy**
* **Jupyter Notebook / Google Colab / VS Code**

---

# 🧪 Experiments

## Experiment 1 — Text Generation Using Pre-trained Foundation Models

### 🎯 Aim

To develop a text generation application using the pre-trained **GPT-2** foundation model.

### 🤖 Model

`gpt2`

### 🔑 Concepts

* Foundation Models
* GPT-2
* Text Generation
* Greedy Search
* Sampling
* Top-k Sampling
* Top-p/Nucleus Sampling
* Temperature

### 📝 Sample Prompt

```text
Artificial Intelligence will transform the future of
```

### 📤 Sample Output

```text
--- Generated Text 1 ---
Artificial Intelligence will transform the future of healthcare, education,
and transportation by enabling smarter decision making and automating
repetitive tasks across industries.

--- Generated Text 2 ---
Artificial Intelligence will transform the future of work by creating new
job roles while automating routine processes in manufacturing and services.
```

### ✅ Result

Text was successfully generated from a given prompt using GPT-2 and sampling-based decoding.

---

# Experiment 2 — Prompt Engineering Techniques

### 🎯 Aim

To implement **zero-shot, few-shot, and chain-of-thought prompting** techniques for content generation, reasoning, and task automation.

### 🔑 Concepts

* Zero-shot prompting
* One-shot prompting
* Few-shot prompting
* Chain-of-thought prompting
* In-context learning

### 📤 Sample Output

```text
=== Zero-shot ===
Sentiment: Positive

=== Few-shot ===
Review: 'The product quality is excellent!'
Sentiment: Positive

=== Chain-of-Thought ===
A: Let's think step by step. 120 - 45 = 75.
75 + 30 = 105. The answer is 105.
```

### ✅ Result

Different prompting techniques were successfully implemented and compared for classification and reasoning tasks.

---

# Experiment 3 — Conversational AI Chatbot

### 🎯 Aim

To build a multi-turn conversational AI chatbot using a transformer-based language model.

### 🤖 Model

`microsoft/DialoGPT-medium`

### 🔑 Concepts

* Conversational AI
* Transformer Models
* Dialogue History
* Multi-turn Conversations
* Context Retention

### 💬 Sample Interaction

```text
Chatbot ready! Type 'quit' to exit.

>> User: Hi, how are you?
Bot: I'm doing great, thanks for asking! How about you?

>> User: What can you help me with?
Bot: I can chat with you about almost anything - just ask away!
```

### ✅ Result

A multi-turn conversational chatbot was successfully developed using DialoGPT.

---

# Experiment 4 — Text Summarization and Question Answering

### 🎯 Aim

To develop a text summarization and question-answering system using pre-trained Transformer models.

### 🤖 Models

**Summarization:**
`facebook/bart-large-cnn`

**Question Answering:**
`distilbert-base-cased-distilled-squad`

### 🔑 Concepts

* Abstractive Summarization
* Extractive Question Answering
* BART
* DistilBERT
* Transformer Architecture

### 📤 Sample Output

```text
Summary:
Generative AI models produce new content such as text, images, audio and video.
Large Language Models are trained on massive text corpora and perform many NLP tasks.

Question: What are Large Language Models trained on?

Answer: massive text corpora | Confidence: 0.87
```

### ✅ Result

Text summarization and question answering were successfully implemented using BART and DistilBERT.

---

# Experiment 5 — Sentiment Analysis and Document Classification

### 🎯 Aim

To perform sentiment analysis and multi-class document classification using pre-trained foundation models.

### 🤖 Models

**Sentiment Analysis:**
`distilbert-base-uncased-finetuned-sst-2-english`

**Zero-Shot Classification:**
`facebook/bart-large-mnli`

### 🔑 Concepts

* Sentiment Analysis
* Text Classification
* Zero-Shot Classification
* Natural Language Inference

### 📤 Sample Output

```text
Review: The new smartphone has an amazing camera and battery life!
-> POSITIVE 0.999

Review: The delivery was late and the packaging was damaged.
-> NEGATIVE 0.998

Document: The central bank raised interest rates to control rising inflation.

Economy: 0.94
Politics: 0.04
Technology: 0.01
Sports: 0.01
```

### ✅ Result

The system successfully identified sentiment polarity and classified a document into the Economy category.

---

# Experiment 6 — Retrieval-Augmented Generation (RAG)

### 🎯 Aim

To build a RAG system that retrieves relevant information from a vector database and generates grounded answers.

### 🛠️ Technologies

* Sentence Transformers
* FAISS
* FLAN-T5
* Vector Embeddings
* Similarity Search

### 🔑 Concepts

* Embeddings
* Vector Databases
* Similarity Search
* Retrieval-Augmented Generation
* Grounded Generation

### 📤 Sample Output

```text
Retrieved Context:
['Retrieval-Augmented Generation combines document retrieval with
text generation.',
 'Vector databases store embeddings and support fast similarity search.']

Answer:
RAG combines document retrieval with text generation using vector databases.
```

### ✅ Result

A RAG system was successfully implemented using FAISS and generated answers using retrieved document context.

---

# Experiment 7 — AI-Powered Code Generation and Debugging Assistant

### 🎯 Aim

To develop an AI assistant that generates code from natural-language instructions and fixes programming errors.

### 🤖 Model

`Salesforce/codegen-350M-mono`

### 🔑 Concepts

* Code Generation
* Code LLMs
* Debugging
* Transformer Decoder Models
* Natural Language to Code

### 📤 Sample Output

```text
Generated Function:

def is_prime(n):
    if n < 2:
        return False
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            return False
    return True
```

### 🐛 Debugging Example

```text
Bug:
result = 0

Fixed:
result = 1
```

### ✅ Result

An AI-powered code generation and debugging assistant was successfully implemented using a pre-trained CodeGen model.

---

# Experiment 8 — Image Generation Using Diffusion Models

### 🎯 Aim

To implement a text-to-image generation application using a pre-trained Stable Diffusion model.

### 🤖 Model

`runwayml/stable-diffusion-v1-5`

### 🔑 Concepts

* Diffusion Models
* Forward Noising
* Reverse Denoising
* Text-to-Image Generation
* Stable Diffusion

### 📝 Sample Prompt

```text
A futuristic city skyline at sunset, digital art, highly detailed
```

### 📤 Output

```text
Image generated and saved as generated_city.png
```

The application generates a **512 × 512 image** based on the given text prompt.

### ✅ Result

A text-to-image generation application was successfully implemented using Stable Diffusion.

---

# 📁 Suggested Project Structure

```text
Generative-AI-Lab/
│
├── README.md
│
├── Experiment-1/
│   └── text_generation.py
│
├── Experiment-2/
│   └── prompt_engineering.py
│
├── Experiment-3/
│   └── chatbot.py
│
├── Experiment-4/
│   └── summarization_qa.py
│
├── Experiment-5/
│   └── sentiment_classification.py
│
├── Experiment-6/
│   └── rag_system.py
│
├── Experiment-7/
│   └── code_generation.py
│
└── Experiment-8/
    ├── image_generation.py
    └── generated_city.png
```

---

# ⚙️ Installation

Install the required libraries using:

```bash
pip install transformers torch
pip install sentence-transformers faiss-cpu
pip install diffusers accelerate
```

For Jupyter Notebook:

```bash
pip install jupyter
```

---

# ▶️ How to Run

### 1. Clone the repository

```bash
git clone <your-repository-link>
```

### 2. Open the project

```bash
cd Generative-AI-Lab
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the required experiment

```bash
python Experiment-1/text_generation.py
```

or open the corresponding notebook in **Jupyter Notebook / Google Colab**.

> **Note:** Experiment 8 requires a CUDA-compatible GPU for practical execution.

---

# 📊 Experiment Summary

| No. | Experiment                  | Main Model/Technology                   |
| --- | --------------------------- | --------------------------------------- |
| 1   | Text Generation             | GPT-2                                   |
| 2   | Prompt Engineering          | GPT-2 / LLM                             |
| 3   | Conversational AI           | DialoGPT                                |
| 4   | Summarization & QA          | BART + DistilBERT                       |
| 5   | Sentiment & Classification  | DistilBERT + BART-MNLI                  |
| 6   | RAG                         | FAISS + Sentence Transformers + FLAN-T5 |
| 7   | Code Generation & Debugging | CodeGen                                 |
| 8   | Image Generation            | Stable Diffusion                        |

---

# 🎓 Learning Outcomes

After completing these experiments, the following concepts are demonstrated:

* Understanding of **Generative AI and Foundation Models**
* Practical use of **Transformer-based models**
* Text generation using **GPT-2**
* Prompt engineering and **in-context learning**
* Development of **conversational AI**
* Text summarization and question answering
* Sentiment and zero-shot classification
* **Retrieval-Augmented Generation**
* Vector embeddings and similarity search
* AI-based code generation and debugging
* Text-to-image generation using **Diffusion Models**

---

# 🏆 Conclusion

These eight experiments provide a practical introduction to modern **Generative AI applications**. They demonstrate how pre-trained foundation models can be applied to text generation, prompt engineering, conversational AI, document understanding, RAG, code generation, and image synthesis without training large models from scratch.

---

## 👩‍💻 Author

**CHANDANA K**
**Computer Science and Engineering (CSE)**

---

⭐ If you find this repository useful, consider giving it a **star**!
