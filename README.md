# Quorum – Your Personal Team of Experts

**Quorum** is an AI-powered Android assistant that gives you instant access to 14 specialized experts in one app. Need legal advice? Emotional support? Help with taxes or relationships? Quorum connects you with the right expert right away.

## 🚀 Key Features

### 🤵 14 Experts in One App
- **Mentor** – Life and career guidance
- **Psychologist** – Emotional support and anxiety relief
- **Assistant** – Task management and voice notes
- **Lawyer** – Civil law, contracts, consumer rights
- **Criminal Lawyer** – Criminal code, court practice
- **Business Coach** – Growth strategies, Lean Canvas, SWOT
- **Love Coach** – Relationships, love languages, compatibility
- **Financial Advisor** – Exchange rates, investments, compound interest
- **Accountant** – Taxes, sole proprietor contributions, tax code
- **Stylist** – Outfit recommendations, color types
- **Wellness Coach** – Habits, sleep, nutrition tracking
- **IT Mentor** – Coding career, interviews, roadmaps
- **Esoteric** – Astrology, numerology, tarot, runes
- **Marketer** – Metrics, audience analysis, promotion strategies

### 👥 Group Chats
Add up to 4 experts to one conversation. Get multiple perspectives on the same question.

### 📄 Smart PDF Reports
Long responses are automatically converted to downloadable PDF reports.

### 🎤 Voice Input
Dictate messages instead of typing.

### 📱 100% Free
No subscriptions. Monetized only through ads (Yandex.Mobile, VK).

## 🛠 Tech Stack

| Component | Technology |
|-----------|------------|
| **Frontend (Android)** | Kotlin + Jetpack Compose |
| **Backend** | Python / FastAPI |
| **Database** | PostgreSQL + pgvector |
| **Cache** | Redis |
| **Embeddings** | BAAI/bge-m3 |
| **LLM** | DeepSeek API |
| **Vector Search** | pgvector (cosine similarity) |
| **TTS** | Yandex SpeechKit |
| **Image Generation** | DALL-E 3 |
| **Ads** | Yandex.Mobile Ads, VK Ads |

## 📁 Project Structure
quorum/
├── android/ # Android app (Kotlin + Compose)
│ ├── app/
│ │ ├── src/main/java/com/example/soul2/
│ │ │ ├── screens/ # UI screens
│ │ │ ├── components/ # Reusable Compose components
│ │ │ ├── utils/ # Helpers (AdManager, etc.)
│ │ │ └── ...
│ │ └── build.gradle
├── backend/ # FastAPI backend
│ ├── app/
│ │ ├── api/ # Endpoints
│ │ ├── adapters/ # RAG adapters for each expert
│ │ ├── calculators/ # Tax, investment calculators
│ │ ├── db/ # Database models
│ │ ├── services/ # Business logic
│ │ └── ...
│ ├── scripts/ # Data loading scripts
│ └── requirements.txt
├── static/ # Privacy policy, terms of service
└── docker-compose.yml

text

## 🧠 How It Works

1. **User asks a question** in a personal or group chat
2. **Backend routes** to the appropriate expert adapter
3. **RAG search** retrieves relevant context from legal codes, tax code, or court practice
4. **LLM generates** a response using DeepSeek API
5. **Response is formatted** and returned to the client
6. **Long responses** are converted to PDF

## 🔐 Monetization

Quorum is **100% free** for users. Revenue comes from:
- **Native ads** in the archetype list
- **Banners** on main screen and chat headers
- **Rewarded video** (users watch ads to get +50 daily messages)

Ad networks: Yandex.Mobile Ads (primary), VK Ads (secondary).

## 📦 Setup

### Prerequisites
- Docker & Docker Compose
- Python 3.12+
- PostgreSQL 16 + pgvector
- Redis 7

### Backend
```bash
cd backend
cp .env.example .env
# Fill in your API keys (DeepSeek, Yandex, etc.)
docker compose up -d
Android
bash
cd android
# Open in Android Studio
# Build and run on device or emulator
📝 Legal
Privacy Policy

Terms of Service

🤝 Contributing
This is a personal project. For suggestions or bug reports, please open an issue.

📧 Contact
Developer: Hayk Virabyan

Email: support@quorum-app.ru

⭐️ License
© 2026 Quorum. All rights reserved.

