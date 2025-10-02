✨ Key Features
📂 Multi-file media group management with PostgreSQL:
media_group
media_queue
chat_histories
📑 Document parsing for CSV, HTML, ICS, JSON, ODS, PDF (with AI fallback), RTF, TXT, XML, and spreadsheets.
🎤 Voice & video transcription for AI analysis.
🖼️ Image, audio, and video description for richer AI context.
🛡️ Telegram-safe MarkdownV2 formatting with auto-splitting for messages over 4096 chars.
⚠️ Error fallback for unsupported file types.
💡 Acknowledgment
A huge thank you to Ezema Gingsley Chibuzo 🙌 for the inspiration of the first version of this workflow:
Create a Multi-Modal Telegram Support Bot with GPT-4 and Supabase RAG
Your pioneering work laid the foundation for this improved, database-powered multi-modal assistant 🚀

🏷 Tags
telegram ai-assistant postgresql multi-file media-group
file-processing voice-transcription document-parser pdf-extraction
markdown-formatting n8n-template

💼 Use Case
Use this template if you need an AI-powered Telegram bot that can:

📦 Handle multiple files sent in a single message (albums, multiple PDFs, etc.).
🧾 Extract & analyze content from many file formats.
🎙️ Transcribe voice and video messages.
🗂️ Maintain chat memory for contextual AI answers.
🛡️ Avoid Telegram formatting errors and length limit issues.
This workflow automates the full chain: Receive → Process → AI Analysis → Telegram-safe Reply.

💬 Example User Interactions
📄 Multiple PDFs with a caption → AI extracts and summarizes all PDFs in one combined reply.
🎤 Voice message → AI transcribes and replies with a contextual answer.
📊 CSV or spreadsheet file → AI parses and summarizes the data.
🖼️ Multiple images → AI describes each image and replies in a single message.
🔑 Required Credentials
Telegram Bot API (Bot Token)
PostgreSQL (Connection credentials)
AI Provider API (OpenAI, Google Gemini, or compatible LLM)
⚙️ Setup Instructions
🗄️ Create the PostgreSQL tables (Gray section SQL):
media_group
media_queue
chat_histories
🔌 Configure the Telegram Trigger with your bot token.
🤖 Connect your AI provider credentials.
🗂️ Set up PostgreSQL credentials in the database nodes.
▶️ Deploy the workflow in n8n.
🎯 Start sending messages and files to your bot.
📌 Extra Notes
✅ Green section ensures only one trigger per media group.
📌 Yellow section guarantees captions and files are stored in the correct sequence.
✨ Purple section formats AI output to be Telegram-safe and split if needed.
🧠 AI prompt is not fixed, allowing full customization.
