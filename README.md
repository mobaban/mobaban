Hey, I'm Mor Baban
AI builder based in Austin, TX.
github.com/mobaban  ·  LinkedIn  ·  mbaban00@gmail.com

I spent a decade in technical sales and engineering in oil and gas and enterprise SaaS. Somewhere along the way I started building AI systems and didn't stop.
I'm not a researcher. I build things that work in production, for real clients, with real constraints. The messy kind of AI work that doesn't look like a tutorial.

What I've Built
AI Property Inspection Platform
Contract engagement, full build
A client needed to automate commercial property inspections. I built the whole system.
Five engines working together: a research engine that pulls zoning data and calculates deadlines automatically, a digital checklist that enforces data integrity (no photo, no submission), a cost engine that fuzzy-matches defects to a pricing database and calculates repair costs, a drafting engine that uses RAG to write professional reports in the client's style, and a rules engine that makes sure nothing ships broken.
The hard part wasn't the AI. It was encoding 20 years of an expert's judgment into rules nobody had written down before.
Stack: Python, Streamlit, Google Gemini, RAG, ChromaDB/FAISS, Pandas, GCP

Medical RAG Assistant
UT Austin GenAI Program
Tested three ways to answer clinical questions: raw LLM, prompt engineering, and RAG over a medical manual.
RAG won. Not just because it was more accurate. Because you could point to exactly which paragraph it used. In healthcare, traceability matters more than a confidence score.
Built the full pipeline: PDF ingestion, chunking, OpenAI embeddings, ChromaDB, retrieval, generation. Evaluated everything with an LLM-as-judge scoring groundedness and relevance.
Stack: Python, LangChain, OpenAI API, ChromaDB

Stock Sentiment Analyzer
UT Austin GenAI Program
NLP pipeline classifying financial news sentiment and correlating it with price movement.
The lesson from this one: 90% accuracy sounds great until you realize your model just predicts the majority class every time. Chose evaluation metrics based on what failure actually costs, not what looks good in a report.
Stack: Python, Pandas, Scikit-learn, NLP

FoodHub Conversational Chatbot
UT Austin GenAI Program
Natural language to SQL. Users ask questions in plain English, the system writes and runs the query, returns a conversational answer. Built prompt templates to handle edge cases where the database just doesn't have what someone asked for.
Stack: Python, LangChain, SQLite, OpenAI API

Tech
AI: LLM orchestration, RAG pipelines, prompt engineering, fine-tuning (PEFT, QLoRA), agentic workflows (LangChain, LangGraph), vector search (FAISS, ChromaDB), computer vision (PyTorch)
Code: Python, JavaScript, TypeScript, React, Next.js, Streamlit
Data: Pandas, Scikit-learn, SQL, PDF and CSV processing
Cloud: AWS, GCP, OpenAI API, Google Gemini API, Hugging Face

Certs
PostGrad in Generative AI for Business Applications, UT Austin McCombs (in progress)
Computer Vision for Data Scientists
Deep Learning and Computer Vision with PyTorch
Google Cybersecurity Certificate
Project Management Foundations

Before All This
I spent 10 years in technical roles where the job was understanding complex systems and translating them into decisions.
At HUVR, a B2B SaaS inspection platform for oil and gas, I ran demos, POC cycles, and discovery calls for enterprise customers. I was the technical bridge between sales and engineering.
At NOV, I was an applications engineer closing $12M+ in equipment deals, working directly with operators on complicated purchasing decisions.
At HP, I deployed enterprise infrastructure for large-scale client environments.
That background matters for how I think about AI. I've been in enough rooms to know the difference between a demo that works and a system that holds up.

Open to roles in solutions engineering, forward-deployed engineering, or applied AI.
mbaban00@gmail.com
