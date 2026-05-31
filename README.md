# 🎮 Player Feedback AI Pipeline (n8n)

## 🚀 Overview

This project is an automated pipeline that collects player feedback from a game UI, processes it using AI, and routes the results to different platforms.

It classifies player messages into:

* **Bug**
* **Feedback**
* **Toxic**

And performs sentiment analysis:

* Positive / Neutral / Negative

## ⚙️ Tech Stack

* n8n (workflow automation)
* OpenAI API (text classification)
* Discord Webhook (alerts)
* Google Sheets API (data storage)

## 🧠 How It Works

1. Player submits feedback from the game
2. Data is sent to n8n webhook
3. AI processes the message:

   * Classifies type (bug / feedback / toxic)
   * Detects sentiment
4. Results are routed:

   * 🚨 Bug → Discord alert
   * 🔥 Toxic → Discord warning
   * 📝 All data → Google Sheets

## 📊 Example Output

```json
{
  "type": "bug",
  "sentiment": "negative"
}
```

## 🖼️ Demo

(Add screenshots or GIF here)

## 📦 Setup

1. Import workflow JSON into n8n
2. Configure environment variables:

   * OPENAI_API_KEY
   * GOOGLE_SHEET_ID
   * DISCORD_WEBHOOK_URL
3. Activate workflow

## 💡 Why This Project?

This project simulates a real-world game analytics tool:

* Helps developers quickly detect bugs
* Filters toxic players
* Collects structured feedback automatically

## 📌 Future Improvements

* Add dashboard (Grafana / Metabase)
* Store data in database (PostgreSQL)
* Real-time analytics
* Player ID tracking

## 👤 Author

Your Name
