# 📬 Smart Email Reply Assistant – Chrome Extension

An AI-powered Chrome Extension that generates smart email replies directly within Gmail using the **Gemini API**.  
Seamlessly integrates into Gmail’s native reply/compose interface — no extra UI needed.

---

## 🚀 Features

- ✨ **AI Reply Button** injected directly into Gmail
- 📄 **Context-Aware**: Sends the current email’s content to the backend for Gemini-powered reply generation
- ⚡ **Instant Insertion**: Generated reply is automatically placed into Gmail’s editable textbox
- 🪶 **Lightweight**: No external UI frameworks, works inside Gmail as-is

---

## 📂 Project Structure

```
smart-email-assistant/
├── email-writer-ext/   # Chrome extension files
├── email-writer-sb/     # Spring Boot backend
└── README.md
```

---

## 🧰 Tech Stack

- **Frontend (Extension)**: JavaScript (Content Scripts), MutationObserver, Fetch API  
- **Backend**: Java, Spring Boot, Gemini API  
- **Browser**: Chrome Extension (Manifest V3)  

---

## 🛠️ Setup Instructions

### 1️⃣ Backend (Spring Boot)
```bash
cd email-writer-sb
./mvnw spring-boot:run
```

### 2️⃣ Load Extension in Chrome
1. Go to `chrome://extensions`
2. Enable **Developer Mode**
3. Click **Load unpacked** and select the `extension/` folder

### 3️⃣ Usage
1. Open **Gmail**
2. Click **Reply**
3. Hit the **AI Reply** button to instantly generate a smart response

---

## 📎 API Endpoint

**POST** `/api/email/generate`  
**Body**:
```json
{
  "emailContent": "string",
  "tone": "professional"
}
```

---

## 📸 Screenshots


---<img width="1918" height="909" alt="Screenshot 2025-08-10 200501" src="https://github.com/user-attachments/assets/192754d0-6013-4f67-bc77-83137cedc5d7" />


<img width="1919" height="908" alt="Screenshot 2025-08-10 200422" src="https://github.com/user-attachments/assets/6be63e66-bd71-4b01-826c-b955b4983f19" />



**Made with ❤️ using Java, Spring Boot, and the Gemini API**
