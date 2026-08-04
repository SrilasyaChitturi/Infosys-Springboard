# 📝 TextMorph-AI – Intelligent Text Processing Platform

TextMorph-AI is a **full-stack NLP application** built during my AI Internship at **Infosys Springboard**, offering multi-model text **summarization, paraphrasing, readability analysis, multilingual translation, and dataset augmentation** — all wrapped in a secure, role-based Streamlit platform with a live admin analytics dashboard.

---

## 🚀 Features

### 👤 User
- Secure registration, login & OTP-based password reset (via email)
- Upload text files or PDFs, or paste text directly
- **Multi-level Summarization** — Short / Medium / Long, across 3 models
- **Advanced Paraphrasing** — adjustable complexity & style (Simplification, Formalization, Creative)
- **Readability Analysis** — Flesch Reading Ease, Flesch-Kincaid, SMOG, Gunning Fog, Coleman-Liau, with visual gauges
- **Multilingual Output** — translate summaries/paraphrases into Hindi, Tamil, Telugu, Kannada, Marathi, Bengali (via NLLB-200)
- Rate & comment on generated outputs (feedback loop)
- Personal **Activity History** of past summarizations/paraphrases
- Editable profile with avatar upload

### 🛡️ Admin
- User management (view, lock/unlock accounts)
- Real-time **Active Users Monitor**
- **Feature Usage Analytics** (Plotly charts)
- **Model Usage & Language Usage Analytics**
- Feedback dashboard with average rating + word cloud of comments
- System-wide **Activity Timeline**

### 🧪 Dataset Augmentation & Model Tuning ("Tune")
- Explore CNN/DailyMail, XSum, and PAWS datasets with live stats
- Interactive data cleaning (min/max word-length filters)
- Configure and simulate fine-tuning runs (architecture, epochs, quantization, batch size, learning rate, dropout)
- Validation report with loss/accuracy metrics

---

## 💡 Key Highlights
- 🤖 **3 interchangeable summarization/paraphrasing models** — FLAN-T5, BART, Pegasus (4-bit quantized for efficient inference)
- 🌐 **NLLB-200 multilingual translation** for output localization
- 🔐 **Bcrypt-hashed passwords**, password-history tracking, and login rate-limiting
- 📧 **SMTP-based OTP email verification** for password recovery
- 📄 **PDF/TXT text extraction** for file-based input (PyPDF2)
- 📊 Real-time **admin analytics dashboard** built with Plotly & word clouds
- 🗂️ Persistent storage via **SQLite**, with Google Drive-backed database for Colab deployments
- ☁️ Deployed live from Google Colab using **Streamlit + ngrok** tunneling

---

## 🧱 Tech Stack

### Frontend / App Framework
- Streamlit
- streamlit-option-menu (sidebar navigation)
- Plotly (data visualization — interactive charts & gauges)
- WordCloud

### NLP / ML
- Hugging Face Transformers (FLAN-T5, BART, Pegasus, NLLB-200)
- PyTorch
- BitsAndBytes (4-bit/8-bit quantization)
- NLTK (sentence tokenization)
- textstat (readability metrics)

### Backend & Data
- SQLite (users, feedback, activity logs, usage analytics)
- Pandas
- Hugging Face Datasets (CNN/DailyMail, XSum, PAWS)

### Authentication & Security
- PyJWT
- bcrypt (password hashing)
- python-dotenv
- SMTP (Gmail) for OTP delivery

### Deployment
- Google Colab (GPU runtime)
- pyngrok (public tunnel for live demo access)

---

## **🔑 Core Pages**
| Page | Description |
|---|---|
| **Summarize** | Multi-model, multi-level text summarization with translation |
| **Paraphrase** | Complexity/style-controlled paraphrasing with translation |
| **Readability** | Text complexity scoring with visual grade-level gauges |
| **Tune** | Dataset exploration + simulated model fine-tuning |
| **History** | Personal log of past generations |
| **Profile** | Avatar, account details |
| **Admin** | Platform-wide analytics, user & feedback management |

## **⚙️ Setup (Colab)**
```bash
pip install streamlit pyjwt bcrypt python-dotenv pyngrok nltk streamlit-option-menu plotly textstat PyPDF2 transformers torch sentencepiece accelerate pandas datasets wordcloud "bitsandbytes>=0.40.0"
```
Add `NGROK_AUTHTOKEN` (and optionally `EMAIL_PASSWORD` for OTP emails) to Colab Secrets, then run the app — a public ngrok URL is generated automatically.

## 🗂️ Project Structure

```text
TextMorph-AI/
├── app.py              # Main Streamlit app — pages, navigation, auth flow
├── engine.py            # Model loading & inference (summarization, paraphrasing, translation)
├── db.py                 # SQLite schema, auth, feedback, activity & usage logging
├── readability.py         # Readability metrics (Flesch, SMOG, Gunning Fog, Coleman-Liau)
└── README.md
