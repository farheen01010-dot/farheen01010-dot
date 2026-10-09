<div align="center">

![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=26&duration=3000&pause=2000&color=6366F1&center=true&vCenter=true&width=900&lines=Hi+%F0%9F%91%8B+I'm+Farheen;AI%2FML+Engineer;Technical+Researcher+in+AI;LLM+Evaluation+%7C+Prompt+Engineering+%7C+RAG)

![Profile Views](https://komarev.com/ghpvc/?username=farheen01010-dot&label=Profile+Views&color=6366f1&style=flat-square)
![Followers](https://img.shields.io/github/followers/farheen01010-dot?label=Followers&style=flat-square&color=6366f1)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/farheen-41a559246)

</div>

---

## 👩‍💻 About Me

**Technical Researcher in Artificial Intelligence** with expertise in **LLM evaluation, prompt engineering, Retrieval-Augmented Generation (RAG) systems, model validation and data analysis**. I assess model performance, analyze model behavior, improve data quality and build scalable AI/ML evaluation pipelines, turning research insights into practical solutions that make AI applications more reliable and accurate.

- 💼 **Role:** Technical Research Associate @ Keywords Studios, Gurugram (Oct 2025 – Present)
- 🎓 **Education:** Bachelor in Biotechnology, Sharda University, Greater Noida (Aug 2021 – Jun 2025)
- 🔍 **What I do:** Prompt engineering, data labeling, LLM evaluation pipelines and SFT data work
- 🏗️ **Latest project:** YouTube RAG Chatbot (LangChain + FAISS + Ollama)
- 🧠 **Currently focused on:** LLM evaluation, advanced RAG and NLP
- 📬 **Reach me:** farheen01010@gmail.com

---

## 💼 Experience Highlights

### Technical Research Associate | Keywords Studios, Gurugram *(Oct 2025 – Present)*
- Reduced LLM errors by **75%** using prompt engineering, data labeling and evaluation pipelines
- Led a team of **8 researchers** and standardized AI evaluation workflows
- Contributed to multiple AI pilot projects involving **Supervised Fine-Tuning (SFT)** of LLMs: data preparation, annotation, QA and evaluation
- Integrated **Chain-of-Thought (CoT)** prompting and structured reasoning traces, improving interpretability by **25%**
- Built **JSON-based action schemas** and tool-invocation validation for reliable agent decision-making
- Performed quality assurance on AI/ML model outputs to surface inconsistencies

### Research Associate | Keywords Studios *(May 2025 – Aug 2025)*
- Annotated and curated large-scale datasets for AI model pre-training and ML pipelines
- Classified structured and unstructured data against strict quality guidelines and client requirements
- Improved training data quality, directly benefiting AI model performance

---

## 🛠️ Tech Stack & Tools

### 💻 Languages
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

### 🤖 AI / ML & LLM
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![CatBoost](https://img.shields.io/badge/CatBoost-FFCC00?style=for-the-badge&logoColor=black)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=for-the-badge&logoColor=white)

### 🧰 Tools & MLOps
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![MS Excel](https://img.shields.io/badge/MS_Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)

### 🧠 Core Skills
`LLMs` `Prompt Engineering` `LLM Evaluation` `RAG` `NLP` `OOPs` `APIs` `Supervised Fine-Tuning (SFT)` `CoT Prompting` `JSON` `Data Annotation` `Dataset Curation`

---
name: Generate Snake Animation

on:
  # runs automatically every 12 hours
  schedule:
    - cron: "0 */12 * * *"
  # lets you run it manually from the Actions tab
  workflow_dispatch:
  # runs when you push to main
  push:
    branches:
      - main

permissions:
  contents: write

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - name: Generate snake from contribution graph
        uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      - name: Push snake to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
---

## 🚀 Featured Projects

### 📺 YouTube RAG Chatbot
> RAG chatbot that answers questions from YouTube video transcripts using semantic search and Llama.

- Retrieves the most relevant transcript chunks with **semantic search (FAISS)**
- Generates grounded answers with a locally run **Llama** model through **Ollama**
- Built with **LangChain** and **Hugging Face** embeddings

**Stack:** `Python` `LangChain` `FAISS` `Hugging Face` `Ollama`

[![GitHub](https://img.shields.io/badge/GitHub-View_Repo-181717?style=flat-square&logo=github)](https://github.com/farheen01010-dot/youtube-rag-chatbot)

---

### 🎙️ Multimodal Student AI Chatbot
> Student assistant with both text and voice interaction.

- **90% accuracy** and **0.90 macro F1-score** across **11 intents**
- Intent classification with **TF-IDF + Logistic Regression**
- Voice input via **SpeechRecognition**, spoken replies via **pyttsx3**
- Confidence-based **unknown-intent detection** and conversation logging

**Stack:** `Python` `NLP` `Scikit-learn` `Streamlit` `SpeechRecognition` `pyttsx3`

[![GitHub](https://img.shields.io/badge/GitHub-View_Repo-181717?style=flat-square&logo=github)](https://github.com/farheen01010-dot/Multimodal_Chatbot)

---

### 💰 Employee Salary Prediction (MLOps)
> End-to-end salary prediction pipeline, from model to deployment.

- Trained a **CatBoost** model for salary prediction
- Served through a **Streamlit** app
- Containerised with **Docker** and automated with **GitHub Actions** (CI/CD)

**Stack:** `Python` `CatBoost` `Streamlit` `Docker` `GitHub Actions`

[![GitHub](https://img.shields.io/badge/GitHub-View_Repo-181717?style=flat-square&logo=github)](https://github.com/farheen01010-dot/Employee_Salary_MLOps)

---

### 📊 More ML Projects
- 🏠 [**House Price Prediction**](https://github.com/farheen01010-dot/House_Price_Prediction): regression model using Linear Regression
- 📉 [**Customer Churn Prediction**](https://github.com/farheen01010-dot/customer-churn-prediction): predicting which customers are likely to leave
- 🎬 [**Movie Recommender**](https://github.com/farheen01010-dot/Movie-Recommender): movie recommendation system

---

## 🎯 Current Focus

- 🧪 Going deeper into **LLM evaluation**: rubrics, benchmarks and quality metrics
- ✍️ Improving **prompt engineering** and reasoning-trace techniques
- 🔎 Building more **RAG** applications
- 🚀 Shipping **production-ready** ML projects with MLOps practices

---

## 📞 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/farheen-41a559246)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:farheen01010@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/farheen01010-dot)

---

<div align="center">

**🤖 Open to AI / LLM opportunities | 🚀 Always learning | 🎯 Focused on practical AI**

</div>
