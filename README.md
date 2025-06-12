Sure! Below is the **complete `README.md` file** — copy and paste it directly into your GitHub repo 👇

---

````markdown
# 🍛 AI-Powered Restaurant Order Automation Bot (n8n + Telegram + Google Sheets)

This is a complete end-to-end automated restaurant ordering system built using **n8n**, **Telegram**, **Google Sheets**, and an **AI Agent** powered by **Google Gemini**. It helps small food businesses manage customer orders, track status, and automate profit reporting — without writing backend code.

---

## 🚀 Features

- 🧾 **Customers place orders via Telegram**
  - View menu
  - Place orders
  - Share name and delivery address

- 🧠 **AI agent handles**
  - Conversation flow
  - Price calculation
  - Order confirmation

- 📄 **Orders are saved in Google Sheets**

- 🛎️ **Restaurant team gets**
  - Order alert on Telegram
  - Inline buttons (Accept, Packed, Delivered)

- 🔁 **Order status updates**
  - Update Google Sheets
  - Notify customers in real-time

- 💰 **Daily at 10 AM**
  - Automatically calculate total earnings
  - Send profit summary to Telegram group

---

## 🧠 Tech Stack

| Tool               | Purpose                             |
|--------------------|--------------------------------------|
| **n8n**            | Workflow automation platform         |
| **Telegram Bot**   | Customer & restaurant communication  |
| **Google Sheets**  | Order storage & profit tracking      |
| **Google Gemini AI**| Handles customer chat logic         |
| **JS Code Node**   | Calculates daily profit              |

---

## 🧰 Project Files

```bash
.
├── README.md                           # Project readme
├── restaurent_bot_final_final.json    # Final n8n workflow export
├── assets/
│   └── workflow.png                   # Optimized visual flow diagram
````

---

## 📷 Live Demo Preview

🎥 \[Insert video link here]
Add a video showing the workflow in action: Telegram chat → AI flow → Google Sheet → Daily profit message

---

## 🛠️ Setup Instructions

1. **Clone the Repo**

```bash
git clone https://github.com/yourusername/restaurant-n8n-bot.git
cd restaurant-n8n-bot
```

2. **Import Workflow into n8n**

* Open n8n → Settings → Import Workflow
* Select `restaurent_bot_final_final.json`

3. **Configure Integrations**

* Set up a Telegram Bot via [@BotFather](https://t.me/botfather)
* Connect your Google Sheets account in n8n
* Ensure your sheet has the following columns:

  ```
  ChatID | CustomerName | DeliveryAddress | OrderedItems | TotalAmount | OrderStatus
  ```
* Add Google Gemini API credentials (for the AI Agent)

4. **Deploy and Test**

* Run the Telegram bot
* Simulate a few orders
* Watch updates in Sheets and Telegram
* Wait until 10 AM (or manually trigger the daily report)

---

## 🔁 How It Works (Flow Summary)

```mermaid
graph TD
A[Customer Telegram Message] --> B[AI Agent]
B --> C[Google Sheets (Save Order)]
C --> D[Send Message to Restaurant Bot]
D --> E[Order Status Button Click]
E --> F[Update OrderStatus in Sheets]
F --> G[Notify Customer via Telegram]
```

---

## 📅 Automations Included

| Event                       | Trigger Node     | Action                                    |
| --------------------------- | ---------------- | ----------------------------------------- |
| New Order from Customer     | Telegram Trigger | AI confirms + saves order to sheet        |
| Staff Updates Order Status  | Telegram Buttons | Sheet is updated + customer notified      |
| Daily Profit Summary @ 10AM | Schedule Trigger | JS sums `TotalAmount` + sends to Telegram |

---

## 🌟 Why This Project?

* No-code/low-code solution
* Minimal maintenance
* AI-enhanced UX
* Works well for small restaurants, cloud kitchens, and food delivery setups

---

## 🧠 Customization Ideas

* Integrate UPI/QR payment verification
* Multi-location restaurant support
* WhatsApp bot version (via Twilio or 360Dialog)
* Firebase or Supabase as database backend

---

## 🤝 Credits

Built by [@Jayanth Kumar](https://www.linkedin.com/in/jayanth-kumar-/)
Powered by open-source tools and automation magic ⚙️✨

---

## 📩 Feedback & Collaboration

If you'd like help deploying this for your own food business or have feature ideas —
📬 DM me on  [LinkedIn](https://www.linkedin.com/in/jayanth-kumar-/)

---

