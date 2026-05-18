# 🎓 Gemma EduBot: Bilingual RAG Tutor for Remote Areas

**A lightweight, 4-bit quantized RAG AI tutor bringing Quantum Physics and English to remote Vietnamese communities without cloud dependency. Submission for the Google Gemma 4 Good Hackathon.**

---

## 🎥 Live Demo & Video Pitch
* **Video Pitch:** https://www.youtube.com/watch?v=dn59ifrXc1Q&t=47s
* **Live Demo:** https://colab.research.google.com/drive/1xUeGQ2fa69Q_kFzrQklCyZylrB1OqGVO?usp=sharing

## 🌍 The Problem: The Digital Divide
In remote areas of Vietnam, students face a significant shortage of expert teachers for advanced subjects like Quantum Physics and essential skills like English communication. High-speed internet is often unstable, making cloud-based AI expensive and inaccessible.

## 💡 The Solution
Gemma_EduBot is a personalized AI tutor designed to run entirely on limited hardware (Edge AI).
* **Factual Accuracy:** Using RAG (Retrieval-Augmented Generation) with FAISS, the bot answers based on a specialized local curriculum, eliminating hallucinations.
* **Bilingual Mastery:** A unique bilingual toggle allows students to switch between Vietnamese and English instantly.
* **Empowering Local Teachers (Admin Panel):** A dedicated Admin Panel allows teachers to easily upload new `.txt` lesson files and rebuild the FAISS Vector Database locally with one click—no coding required.

## ⚙️ Technical Architecture
* **Core Model:** Google's **Gemma-2b-it**
* **Optimization:** **4-bit quantization (bitsandbytes)** to ensure the model runs on edge devices or free-tier GPUs (~2.5GB VRAM).
* **RAG Pipeline:** **LangChain** and **FAISS** for fast semantic search.
* **UI:** **Streamlit** for a lightweight, user-friendly interface.

*Note: The model weights are not included in this repository due to file size limits. They will be downloaded automatically when running the application via Colab.*

## 🚀 How to Run (Live Demo)
Because this RAG system requires a T4 GPU and 4-bit Quantization, the easiest way to test this project is via our provided Google Colab notebook:
1. Open the Live Demo Google Colab link above.
2. Click `Runtime` -> `Run all`.
3. Scroll to the bottom to get the Endpoint IP password.
4. Click the generated Localtunnel link and paste the password to access the Streamlit UI.
