# Gemini Study Buddy Bot: AI-Powered Q&A and Quiz Assistant

An interactive **Gemini 2.0 Flash Lite-powered Study Buddy Bot** designed to help you learn effectively by:
✅ Answering your questions in a conversational flow.  
✅ Generating quizzes for active recall and practice.  
✅ Ingesting your course notes directly from **Google Drive PDFs** using **PyMuPDF**.

---

## 🚀 Features

✅ **Rule-Based Menu** for seamless offline navigation:
- Choose between `midterm` and `final` study modes.
- `ask` to start Q&A sessions.
- `quiz` to practice quizzes.
- `bye` to exit.

✅ **Google Drive Mount + PyMuPDF Ingestion**:
- Automatically extract course notes from PDFs.
- Organize files cleanly between midterm and final contexts.

✅ **Gemini-Powered Q&A (`handle_ask`)**:
- Uses **Gemini chat history** for flowing conversations.
- Students can ask multiple consecutive questions while maintaining context.
- Provides clear, concise explanations using course notes or external knowledge.

✅ **Gemini-Powered Quizzes (`handle_quiz`)**:
- Generates **one quiz question at a time with hidden answers for validation**.
- Uses Gemini to check correctness and provide explanations if the answer is incorrect.

---

## 🛠️ Technical Details

- **Gemini 2.0 Flash Lite**:
  - Fast, instruction-following outputs.
  - Strong technical explanations for courses like AI, Networking, and OS.
  - Handles large context windows for entire course notes.
  - Free plan supports 200 requests/day for focused study sessions.

- **PyMuPDF**:
  - Efficient, lightweight PDF extraction for clean text processing.
  - Supports automated context ingestion directly from Google Drive.

---

## 🚩 Limitations

- **200 queries/day** on Gemini free plan; heavy study sessions may approach this limit.
- Extremely large PDFs may require pre-summarization or retrieval chunking.
- Gemini-based correctness evaluation; advanced fuzzy matching could enhance grading.

---

## 📂 Setup and Usage

1️⃣ **Clone this repository**:
```bash
git clone https://github.com/yourusername/gemini-study-buddy-bot.git
cd gemini-study-buddy-bot
