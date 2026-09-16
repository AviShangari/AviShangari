# Hi, I'm Aaveg Shangari

Backend and full-stack engineer with an applied ML focus. B.Sc. Honours Computer
Science from Ontario Tech (3.87 GPA, Highest Distinction). I build systems that
run in production, not notebooks.

Currently looking for backend, full-stack, or applied ML roles in Canada.

## What I'm Working On

### [Savvant](https://savvant.ca) — Canadian personal finance, built solo

A production personal finance platform that links real Canadian bank accounts
through Plaid, syncs transactions and liabilities continuously over verified
webhooks, and learns how each user categorizes their own spending.

**Engineering worth mentioning:**

- **Deterministic chatbot.** GPT-4o-mini classifies intent and formats prose;
  a Python engine computes every figure. The model never does arithmetic on
  your money. Freeform questions go through a generated SELECT that is
  validated before execution: read-only, single-table, user-scoped as a bound
  parameter, capped results.
- **Per-user ML categorization.** LightGBM over character n-gram TF-IDF plus
  amount, recurrence, and temporal features, trained only on that user's own
  verified labels and retrained on every correction. Non-text features exist
  because Plaid merchant names collide (every Apple charge arrives as "Apple").
- **Double-count-proof taxonomy.** Plaid issues a new transaction id when a
  pending charge posts. Detected via `pending_transaction_id` and promoted in
  place, preserving user corrections, so nothing is counted twice.
- **Production integration.** Fernet-encrypted access tokens, verified ES256
  JWT webhooks, cursor-based sync with per-row error isolation.

**Stack:** FastAPI · PostgreSQL · SQLAlchemy · Alembic · Plaid · LightGBM ·
scikit-learn · React · Docker · Railway

*Source is private — it is a live application handling real financial data.
Happy to walk through the architecture or share access on request.*

**[Try it live →](https://savvant.ca)**

---

### [ParaTracker](https://github.com/vclab/worm-tracker) — C. elegans motion analysis

Computer vision system built at Ontario Tech's Visual Computing Lab, used by
the biology department on their own experiments. I built the core tracking
pipeline (skeletonization plus Hungarian matching, 85%+ identity consistency),
trained a custom YOLOv8-seg model that cut redundant track IDs roughly 80% over
the classical approach, and packaged the whole thing as a standalone Windows
application so researchers run it without touching a command line.

**Stack:** PyTorch · Ultralytics YOLOv8-seg · OpenCV · scikit-image · FastAPI ·
React · SQLite

---

### [BravoBot](https://github.com/AviShangari/Bravobot-Voice-Assistant) — offline voice assistant

Local-first voice assistant. Whisper for speech-to-text, fine-tuned DistilBERT
across 13 intents, Llama 3.2 for generation, FAISS semantic memory over 384-dim
sentence embeddings. Everything runs on-device.

**Stack:** Python · Whisper · DistilBERT · FAISS · Ollama · Llama 3.2 · SQLite

## Tech I Work With

**Languages:** Python, Java, C++, JavaScript, SQL, Bash
**Backend & Data:** FastAPI, PostgreSQL, SQLAlchemy, Alembic, Docker, Railway
**AI/ML:** scikit-learn, PyTorch, LightGBM, OpenCV, FAISS, SentenceTransformers
**Frontend:** React, Tailwind CSS, Vite

## Let's Connect

📧 shangariaaveg@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/aaveg-shangari/) ·
[Portfolio](https://avishangari.github.io/aaveg-portfolio/)
