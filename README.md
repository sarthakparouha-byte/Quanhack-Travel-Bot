# ✈️ QuanTravel AI — AI Travel Itinerary Assistant

> **QuAnHack Internship Final Round Submission**
> Problem Statement: Travel Agencies — AI Itinerary Assistant

---

## 🚀 Live Demo

> Open `index.html` in any browser — no installation, no backend, no setup needed.

---

## 📌 What It Does

QuanTravel AI is a WhatsApp-style conversational AI assistant that helps travel agencies automate their enquiry and lead capture process.

A user chats with the bot, answers 4 simple questions, and receives a fully personalized AI-generated travel itinerary — all within seconds. The lead is captured, stored, and a real confirmation email is sent to the user's inbox automatically.

---

## 🔄 Workflow

```
User Input → Guided Chat Flow → Gemini API → Itinerary Output
                                                     ↓
                                            User says yes?
                                                     ↓
                                          Lead Capture Form
                                           ↙            ↘
                                    localStorage      EmailJS
                                         ↓               ↓
                                     CSV Export    Confirmation
                                                    Email Sent
```

---

## ⚙️ How It Works

1. User opens the app and is greeted by the QuanTravel AI bot
2. Bot guides the user through 4 questions — destination, duration, budget, and interests
3. Full conversation is sent to **Google Gemini API** which generates a day-by-day itinerary
4. Itinerary is displayed in chat with a **Download as .txt** option
5. Bot asks if the user wants a travel expert to reach out
6. If yes — lead form is filled and submitted
7. **EmailJS** fires a real confirmation email to the user's inbox
8. Lead is saved to **localStorage** and exportable as **CSV**

---

## ✨ Features

| Feature | Description |
|---|---|
| 💬 WhatsApp-style UI | Familiar chat interface with message bubbles, timestamps, and blue ticks |
| 🤖 AI Itinerary Generation | Google Gemini generates detailed day-by-day travel plans |
| ⚡ Quick Reply Chips | Contextual suggestion buttons after every bot message |
| 📧 Real Email Confirmation | EmailJS sends actual email to user inbox on form submit |
| 💾 Lead Management | All leads saved in localStorage, viewable in modal table |
| 📤 CSV Export | Download all captured leads as a CSV file in one click |
| 📄 Itinerary Download | Save AI-generated plan as a .txt file via Blob API |
| 📱 Mobile Responsive | Works on all screen sizes |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML5 + CSS3 + Vanilla JavaScript |
| AI Engine | Google Gemini API (gemini-flash-latest) |
| Email Service | EmailJS |
| Data Storage | Browser localStorage |
| File Export | Blob API |
| Fonts | Google Fonts (Inter) |

---

## 🗂️ Project Structure

```
quanhack-travel-ai/
├── index.html      ← Complete app (single file)
└── README.md       ← This file
```

---

## 🏃 How To Run

1. Clone or download this repo
2. Add your API keys inside `index.html`:
   ```javascript
   const API_KEY = "YOUR_GEMINI_API_KEY";
   ```
   And your EmailJS credentials:
   ```javascript
   emailjs.init("YOUR_PUBLIC_KEY");
   ```
3. Open `index.html` in any browser
4. That's it — no npm install, no server needed

---

## 🔮 Future Scope

- Integrate with **WhatsApp via Twilio / WATI** for real messaging
- Connect leads to **HubSpot / Zoho CRM** for sales pipeline management
- Add a **backend (Firebase / Node.js)** for cross-device lead persistence
- Build a **travel agent dashboard** to manage and follow up on leads
- Add **payment gateway** for instant package booking from chat
- Extend to other domains — Medical Lab Booking, Education Enquiry Assistant

---

## 💡 Problem It Solves

Travel agencies waste hours daily answering repetitive enquiries. QuanTravel AI automates the entire initial conversation, generates a personalised itinerary, captures the lead, and sends a confirmation email — all without human involvement. This reduces response time from hours to seconds and lets agents focus only on closing bookings.

---

## 👤 Submitted By

Sarthak Parouha
QuAnHack Solution Internship Final Round — AI Workflow Challenge
