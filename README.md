Hey, I'm Mor Baban
AI builder based in Austin, TX.
github.com/mobaban  ·  [LinkedIn](https://www.linkedin.com/in/babanm/)  ·  mbaban00@gmail.com

I spent a decade in technical sales and engineering in oil and gas and enterprise SaaS. Somewhere along the way I started building AI systems and didn't stop. I'm not a researcher. I build things that work in production, for real clients, with real constraints. The messy kind of AI work that doesn't look like a tutorial.

## What I've Built

**AI Property Inspection Platform** | Contract engagement, full build, solo, under 5 months

A client in the inspection and assessment space needed to automate commercial property condition assessments, the reports banks require before real estate deals close. I designed and shipped the whole system end to end: architecture, data model, AI orchestration, deployment.

The core principle: the AI is never the source of truth. The system controls the workflow, the model does bounded generation inside it, and every claim the model produces gets verified before a human sees it.

- **Research automation:** four government hazard APIs (FEMA, EPA, NOAA, NRCS) pulled in parallel instead of sequentially, every response sourced and timestamped for a full provenance chain. Two hours of desk research down to under a minute.
- **Vision-assisted field capture:** inspectors upload site photos, Gemini vision proposes findings mapped to the right building component. The inspector reviews, accepts, or overrides every one, nothing ships without sign-off.
- **RAG-grounded report drafting:** generation is grounded in the firm's own reference documents, not the model's training data.
- **The validation layer:** every factual claim in a generated report gets extracted and cross-checked against the actual structured input. If the model invents a number, there's nothing to trace it to, so it gets caught before it ever reaches a client. This is the part I'm most proud of, not the generation, but the layer that assumes the model will sometimes be confidently wrong and catches it.
- **Auto-costed findings and reserve schedules**, matched against the firm's own cost library, calculated over a multi-year horizon with inflation factored in.
- **Multi-tenant architecture** with five-tier role-based access control, so one client's data can never touch another's.

Stack: Python, Streamlit, Google Gemini, LangChain, LangGraph, RAG, ChromaDB/FAISS, Firestore, Cloud Storage, Docker, GitHub Actions CI/CD, GCP Cloud Run

---

**Medical RAG Assistant** | UT Austin Data Science / GenAI Postgrad

Tested three ways to answer clinical questions: raw LLM, prompt engineering, and RAG over a medical manual. RAG won. Not just because it was more accurate. Because you could point to exactly which paragraph it used. In healthcare, traceability matters more than a confidence score. Built the full pipeline: PDF ingestion, chunking, OpenAI embeddings, ChromaDB, retrieval, generation. Evaluated everything with an LLM-as-judge scoring groundedness and relevance.

Stack: Python, LangChain, OpenAI API, ChromaDB

---

**Stock Sentiment Analyzer** | UT Austin Data Science / GenAI Postgrad

NLP pipeline classifying financial news sentiment and correlating it with price movement. The lesson from this one: 90% accuracy sounds great until you realize your model just predicts the majority class every time. Chose evaluation metrics based on what failure actually costs, not what looks good in a report.

Stack: Python, Pandas, Scikit-learn, NLP

---

**FoodHub Conversational Chatbot** | UT Austin Data Science / GenAI Postgrad

Natural language to SQL. Users ask questions in plain English, the system writes and runs the query, returns a conversational answer. Built prompt templates to handle edge cases where the database just doesn't have what someone asked for.

Stack: Python, LangChain, SQLite, OpenAI API

## Tech

**AI:** LLM orchestration, RAG pipelines, prompt engineering, fine-tuning (PEFT, QLoRA), agentic workflows (LangChain, LangGraph), vector search (FAISS, ChromaDB), computer vision (PyTorch)

**Code:** Python, JavaScript, TypeScript, React, Next.js, Streamlit

**Data:** Pandas, Scikit-learn, SQL, PDF and CSV processing

**Cloud:** GCP (Cloud Run, Firestore, Cloud Storage), AWS, Docker, GitHub Actions CI/CD, OpenAI API, Google Gemini API, Hugging Face

## Certs

- Project Management Professional (PMP), PMI, 2025
- Postgraduate Program, Generative AI for Business Applications, UT Austin McCombs School of Business (Mar 2024 – Mar 2026, completed)
- Google Cybersecurity Professional Certificate, Google
- Computer Vision for Data Scientists
- Deep Learning and Computer Vision with PyTorch
- Project Management Foundations

## Before All This

I spent 10 years in technical roles where the job was understanding complex systems and translating them into decisions.

At HUVR, a B2B SaaS inspection platform for oil and gas, I ran demos, POC cycles, and discovery calls for enterprise customers. I was the technical bridge between sales and engineering, and drove a 45% utilization increase across my accounts by finding and fixing real workflow friction.

At NOV, I was an applications engineer supporting $12M+ in equipment deals, working directly with drilling and completions teams on complicated technical purchasing decisions. That's also where the oil and gas domain knowledge comes from, a BS in Petroleum Engineering and years of being the technical credibility in the room with engineers who don't tolerate someone who doesn't understand the work.

At HP, I deployed enterprise infrastructure for large-scale client environments.

That background matters for how I think about AI. I've been in enough rooms to know the difference between a demo that works and a system that holds up.

## Open To

Solutions engineering, forward-deployed engineering, applied AI, or roles at the intersection of AI and oil & gas / energy, where the domain background and the build experience compound.

mbaban00@gmail.com
