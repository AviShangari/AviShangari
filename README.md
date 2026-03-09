# Hi, I'm Aaveg Shangari

CS graduate from Ontario Tech (3.89 GPA, Distinction) with a focus on backend engineering, ML systems, and computer vision. I like building tools that solve real problems. My most recent project is a deployed financial intelligence platform that parses real Canadian bank statements using ML.

## What I'm Working On

### [Savvant](https://savvant.ca) — Behavioral Financial Intelligence Platform
A full-stack platform that transforms bank and credit card statements into personalized spending intelligence. No bank linking required — just upload a PDF.

**What's under the hood:**
- Categorization priority chain: manual overrides → LightGBM + TF-IDF (>70% confidence gate) → rule-based fallback
- Hallucination-resistant chatbot: LLM intent classification → Python calculation engine → LLM response formatting
- 16 behavioral spending tags with confidence scoring and adaptive thresholds
- Isolation Forest anomaly detection with per-category feature engineering
- Modular parser registry supporting TD, RBC, and Visa statement formats

**Built with:** FastAPI · PostgreSQL · React · Scikit-learn · LightGBM · Docker

🔗 **[Try it live →](https://savvant.ca)**

---

### Other Projects

**Worm Tracking Thesis** — Novel multi-object tracking pipeline for microscopic organisms using skeletonization + Hungarian Algorithm. Built as a Research Assistant at Ontario Tech's Visual Computing Lab. Includes a FastAPI + React delivery system for non-technical researchers.

**BravoBot** — Offline voice assistant integrating Whisper (STT), fine-tuned DistilBERT (intent classification), and Llama 3.2 (response generation). Designed for privacy-first, local-only inference.

## Tech I Work With

**Languages:** Python, Java, C++, JavaScript, SQL, Bash  
**Backend & Data:** FastAPI, PostgreSQL, SQLAlchemy, Alembic, Docker  
**AI/ML:** Scikit-learn, PyTorch, TensorFlow, OpenCV, LightGBM, FAISS, SentenceTransformers  
**Frontend:** React, Tailwind CSS

## Let's Connect

📧 shangariaaveg@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/aaveg-shangari/) · [Portfolio](https://avishangari.github.io/aaveg-portfolio/)
