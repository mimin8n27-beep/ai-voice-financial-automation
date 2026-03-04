# ai-voice-financial-automation
AI-powered voice-to-structured financial automation system using n8n, LLM parsing, and Google Sheets integration.
AI Voice Financial Automation
📌 Overview

This system automates financial data processing from Telegram voice messages.

It transcribes audio, extracts structured financial data using AI, validates the output, and logs results into Google Sheets automatically.

🏗 System Architecture

Telegram Trigger
→ Voice Download
→ Speech-to-Text
→ AI Parsing (LLM)
→ JavaScript Validation Layer
→ Structured JSON Extraction
→ Google Sheets Logging

⚙ Tech Stack

n8n

Telegram Bot API

Speech-to-Text API

LLM (Gemini / Groq / OpenAI)

Google Sheets API

Custom JavaScript Validation

Error Handling & Retry Logic

🔍 Key Features

Automatic voice transcription

AI-based financial entity extraction

Multi-amount aggregation in single voice note

Clean JSON structuring

Data validation before insertion

Real-time sheet updates

🧩 Technical Challenges Solved

Handling Arabic dialect variations

Parsing multiple financial entries from one voice input

Preventing malformed JSON responses from LLM

Managing API rate limits

Ensuring idempotent logging in Google Sheets

📊 Sample Output
{
  "date": "2026-02-10",
  "category": "Transport",
  "amount": 200,
  "description": "Uber ride"
}
🚀 Impact

Eliminated manual financial logging

Reduced human error by ~90%

Enabled real-time expense tracking

## Project Structure
/docs        → Architecture diagrams, workflow screenshots, and sample outputs  
/workflow    → Exported n8n automation workflow (JSON)
