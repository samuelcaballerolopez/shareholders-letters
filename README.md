# 🏦 Shareholder Letter RAG Analyst

![Google Cloud](https://img.shields.io/badge/Google_Cloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)
![Vertex AI](https://img.shields.io/badge/Vertex_AI-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_2.0_Flash-8E75B2?style=for-the-badge)

An enterprise-grade **Retrieval-Augmented Generation (RAG)** system built on **Google Cloud Vertex AI** and **Gemini 2.0 Flash**, specifically designed to audit, analyze, and extract strategic insights from **Shareholder Letters**.

Unlike basic RAG implementations that simply chunk text, this architecture leverages **Vertex AI Search (Discovery Engine)** to understand the unique narrative structure of Shareholder Letters, ensuring "surgical precision" when retrieving specific executive insights, strategic risks, or tax disputes buried in the text.

---

## 🚀 Key Features

* **☁️ Cloud-Native Architecture:** Fully deployed on Google Cloud Platform (GCP) for security and scalability.
* **🔎 Deep Retrieval:** Uses `extractive_content_spec` to force the search engine to return precise narrative fragments from the letters, avoiding empty metadata results.
* **🧠 SOTA LLM:** Powered by **Gemini 2.0 Flash** for high-speed, low-latency synthesis of executive commentary.
* **📉 Shareholder Narrative Analysis:** Capable of ingesting complex PDF letters (Tesla, Netflix, Berkshire Hathaway) and extracting structured strategic insights.
* **💬 Interactive Interface:** Includes a Python-based interactive chat loop optimized for Google Colab.

---

## 🛠️ Tech Stack

| Component | Technology | Purpose |
| :--- | :--- | :--- |
| **Infrastructure** | Google Cloud Platform | Scalable serverless environment. |
| **Storage** | Cloud Storage (GCS) | Data Lake for raw PDF ingestion (Shareholder Letters). |
| **Retrieval Engine** | Vertex AI Search | Semantic search with OCR and structural understanding. |
| **Generative Model** | Gemini 2.0 Flash | Context synthesis and reasoning. |
| **Orchestration** | Python (Vertex SDK) | Logic handling and API connectivity. |
| **Environment** | Google Colab | Development and testing notebook. |

---

## 📸 Demo

**1. Surgical Precision:**
*The system correctly identifies a specific $619M tax dispute in Brazil buried within Netflix's shareholder letter, ignoring generic tax tables.*

<img width="1839" height="532" alt="output_colab" src="https://github.com/user-attachments/assets/b22e5d71-fddb-4c5b-aebe-2a3866d5fc0f" />


**2. Cloud Infrastructure:**
*Shareholder letters indexed and processed in Vertex AI Agent Builder.*

<img width="1907" height="851" alt="app_cloud" src="https://github.com/user-attachments/assets/a95cfa87-1cc2-4a2f-be53-97a69755b8a7" />


---

## ⚙️ How to Run

This code is optimized for **Google Colab**.

### Prerequisites
1.  A **Google Cloud Platform** project with billing enabled.
2.  Enable the following APIs:
    * `Vertex AI API`
    * `Discovery Engine API` (Vertex AI Search)
3.  Create a **Data Store** in Vertex AI Search and upload your Shareholder Letters (PDFs).

### Setup in Colab
1.  Download the `.ipynb` file from this repository.
2.  Upload it to [Google Colab](https://colab.research.google.com/).
3.  Update the configuration variables (Project ID, Data Store ID) in the second cell of the notebook.
4.  Run the cells. The script will handle authentication via your Google account.

---

## 🧠 Design Decisions

### Why Vertex AI Search instead of local Vector DBs?
* **Scalability:** The system scales automatically from 3 letters to 100,000 without managing servers or re-indexing pipelines.
* **Document Understanding:** Vertex AI parses the native structure of PDFs (headers, columns), which is critical for financial narratives where context is often positional.

### Why "Surgical Precision"?
The system is tuned for specific queries (e.g., *"What strategic risks does Tesla mention?"*) rather than generic summarization. This avoids the "lost in the middle" phenomenon common in LLMs when processing dense executive reports.


---

## 📬 Contact

Created by **Samuel Caballero** - Data Analyst & AI Engineer.

If you have any questions about the architecture or want to discuss AI integration in Finance, feel free to reach out!

<a href="https://www.linkedin.com/in/samuelcablop/" target="_blank">
  <img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
<a href="mailto:samuelcablop@gmail.com">
  <img src="https://img.shields.io/badge/Email-Contact_Me-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
</a>
