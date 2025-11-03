
# 🧠 Domain-Tuned LLM with LoRA (TinyLlama)

Fine-tuning a lightweight open-source LLM on your documents for domain-specific Q&A

This project demonstrates how to fine-tune a TinyLlama 1.1B Chat model using LoRA (Low-Rank Adaptation) on your own PDF/TXT documents to build a private, domain-specialized AI assistant.

✅ Upload any domain document

✅ Auto-extract text & generate Q&A pairs

✅ Fine-tune TinyLlama efficiently

✅ Deploy a chat UI using Streamlit

✅ Works locally / on Colab

✅ No cloud vendor lock-in

⸻

🚀 Features

Capability	Description
📄 Document ingestion	Upload PDFs/TXT for training
🤖 Synthetic Q&A generation	LLM auto-creates training pairs
⚡ Efficient LoRA training	1B model, k-bit + PEFT
🧪 Domain-aware responses	Answers only from your document
🖥️ Chat interface	Streamlit chatbot included
🔐 Private & local	No data leaves your environment


⸻

📦 Tech Stack
	•	🤗 Transformers
	•	🦙 TinyLlama 1.1B Chat
	•	🧠 LoRA + PEFT
	•	⚙️ 8-bit quantization (k-bit training)
	•	🐍 Python
	•	🎨 Streamlit UI

⸻

💡 Why LoRA + TinyLlama?

Benefit	Reason
🚀 Fast	Train in under an hour on Colab T4/A100
💾 Small	Only ~1B params — deployable anywhere
💰 Cheap	No high-end hardware required
🔒 Private	Fine-tune locally, no data sharing
📎 Flexible	Drop-in replacement for SaaS models


⸻

🛠️ Training Workflow

1️⃣ Upload a document

Reads PDF/TXT and extracts text.

2️⃣ Auto-generate Q&A dataset

Uses LLM to create domain-grounded questions.

3️⃣ Format & tokenize prompts

Uses TinyLlama chat format:

<|user|> question
<|assistant|> answer

4️⃣ Fine-tune using LoRA

Low-rank adapters → fast + lightweight.

5️⃣ Chat Interface

Real-time Q&A from your tuned model.

⸻

▶️ Run the Chatbot

streamlit run streamlit_lora_app.py

Then open the browser URL to chat with your fine-tuned model.

⸻

📊 Evaluation Approach
	•	Manual benchmark on held-out questions
	•	Context-fidelity evaluation
	•	Hallucination check
	•	Qualitative response accuracy

⸻

🔥 Results

✔️ Strong domain recall
✔️ Improved factual accuracy
✔️ Very low hallucination rate (after format fix)
✔️ Fast inference on GPU / Colab




