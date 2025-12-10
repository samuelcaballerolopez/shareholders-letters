# 🏦 Financial RAG Analyst (Vertex AI & Gemini)

![Google Cloud](https://img.shields.io/badge/Google_Cloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)
![Vertex AI](https://img.shields.io/badge/Vertex_AI-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_2.0_Flash-8E75B2?style=for-the-badge)

An enterprise-grade **Retrieval-Augmented Generation (RAG)** system built on **Google Cloud Vertex AI** and **Gemini 2.0 Flash**, specifically designed to audit, analyze, and extract strategic insights from **Shareholder Letters**.

Unlike basic RAG implementations that simply chunk text, this architecture leverages **Vertex AI Search (Discovery Engine)** to understand the unique narrative structure of Shareholder Letters, ensuring "surgical precision" when retrieving specific executive insights, strategic risks, or tax disputes buried in the text.
---

## 🚀 Key Features

* **☁️ Cloud-Native Architecture:** Fully deployed on Google Cloud Platform (GCP) for security and scalability.
* **🔎 Deep Retrieval:** Uses `extractive_content_spec` to force the search engine to return precise narrative fragments, avoiding empty metadata results.
* **🧠 SOTA LLM:** Powered by **Gemini 2.0 Flash** for high-speed, low-latency financial synthesis.
* **📉 Unstructured Data Analysis:** Capable of ingesting complex PDFs (Tesla, Netflix, Berkshire Hathaway) and extracting structured insights.
* **💬 Interactive Interface:** Includes a Python-based interactive chat loop optimized for Google Colab.

---

## 🛠️ Tech Stack

| Component | Technology | Purpose |
| :--- | :--- | :--- |
| **Infrastructure** | Google Cloud Platform | Scalable serverless environment. |
| **Storage** | Cloud Storage (GCS) | Data Lake for raw PDF ingestion. |
| **Retrieval Engine** | Vertex AI Search | Semantic search with OCR and structural understanding. |
| **Generative Model** | Gemini 2.0 Flash | Context synthesis and reasoning. |
| **Orchestration** | Python (Vertex SDK) | Logic handling and API connectivity. |
| **Environment** | Google Colab | Development and testing notebook. |

---

## 📸 Demo

**1. Surgical Precision:**
*The system correctly identifies a specific $619M tax dispute in Brazil buried within Netflix's shareholder letter, ignoring generic tax tables.*

![Chat Output](output_colab.png)
<img width="1839" height="532" alt="output_colab" src="https://github.com/user-attachments/assets/6779229c-cefb-42dd-b89b-a5dbadc77d03" />


**2. Cloud Infrastructure:**
*Documents indexed and processed in Vertex AI Agent Builder.*

![Vertex AI Console](Captura_de_pantalla_2025-12-10_084750.png)
<img width="1907" height="851" alt="app_cloud" src="https://github.com/user-attachments/assets/ac418d4c-d0e4-4611-ab1c-ce710f078603" />


---

## ⚙️ How to Run

This code is optimized for **Google Colab**.

### Prerequisites
1.  A **Google Cloud Platform** project with billing enabled.
2.  Enable the following APIs:
    * `Vertex AI API`
    * `Discovery Engine API` (Vertex AI Search)
3.  Create a **Data Store** in Vertex AI Search and upload your PDF documents (e.g., Shareholder Letters).



## 📬 Contact

Created by **Samuel Caballero** 

If you have any questions about the architecture or want to discuss AI integration in Finance, feel free to reach out!

<a href="https://www.linkedin.com/in/samuelcablop/" target="_blank">
  <img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
