# 🤖 WhatsApp AI Agent & Auto-Training System (n8n Workflow)

[![n8n](https://img.shields.io/badge/Otomasi-n8n-FF6D5A?style=for-the-badge&logo=n8n)](https://n8n.io)
[![OpenAI](https://img.shields.io/badge/AI-GPT--4o--mini-41ADFF?style=for-the-badge&logo=openai)](https://openai.com)
[![WhatsApp](https://img.shields.io/badge/Platform-WhatsApp%20Business-25D366?style=for-the-badge&logo=whatsapp)](https://business.whatsapp.com/)

Sistem AI Agent cerdas berbasis **n8n** yang mampu menangani Customer Service secara otomatis melalui WhatsApp. Dilengkapi dengan fitur **Auto-Learning** hanya dengan mengirimkan URL produk!

## 🚀 Fitur Unggulan

* **Multimodal Input:** Mendukung pesan teks dan **Voice Notes** (Otomatis transkripsi via OpenAI Whisper).
* **Auto-Training System:** Kirim pesan format `Train: [URL]` dan AI akan otomatis melakukan *web scraping* untuk mempelajari detail produk Anda.
* **Knowledge Base Integration:** Semua data produk disimpan dan dibaca langsung dari **Google Sheets**.
* **Smart Memory:** AI memiliki ingatan jangka pendek (*Window Buffer Memory*) untuk menjaga konteks percakapan tetap nyambung.
* **Agentic Tools:** AI dapat diperintah untuk mengirim email melalui Gmail secara otomatis.

## 🛠️ Persyaratan Sistem

Sebelum melakukan import, pastikan Anda memiliki akses ke:
1.  **n8n Instance** (Self-hosted via Docker/NPM atau n8n Cloud).
2.  **OpenAI API Key** (Minimal model GPT-4o-mini).
3.  **WhatsApp Business Cloud API** (Meta Developer).
4.  **Google Cloud Console** (Untuk akses Google Sheets & Gmail API).

## 📂 Cara Instalasi

1.  **Clone / Download** file `workflow.json` dari repositori ini.
2.  Buka dashboard **n8n** Anda.
3.  Buat workflow baru, lalu **Copy & Paste** isi file JSON tersebut langsung ke kanvas n8n.
4.  Konfigurasi ulang **Credentials** untuk setiap node:
    * WhatsApp Business API
    * OpenAI API
    * Google Sheets OAuth2
    * Gmail OAuth2
5.  Sesuaikan ID Google Sheets Anda pada node-node terkait.
6.  Klik **Execute Workflow** untuk memulai testing.

## 📊 Struktur Database (Google Sheets)
Pastikan Google Sheet Anda memiliki header berikut di Sheet1:
| Product Link | Product Name | Product Price | Product Topic | Product Description |
| :--- | :--- | :--- | :--- | :--- |
