# 📱 QR Code Generator

A simple and instant QR Code Generator web app built with pure HTML, CSS, and JavaScript. Enter any text or URL and get a scannable QR code in one click — powered by the QR Code API. Deployed live on Vercel.

## 🌐 Live Demo

🔗 **[person-age-calculator-jv9f.vercel.app](https://person-age-calculator-jv9f.vercel.app)**

---

## ✨ Features

- 🔤 **Text & URL Support** — Generate QR codes for any text, link, phone number, email, or any string
- ⚡ **Instant Generation** — Click "Generate QR Code" and QR appears immediately
- 🖼️ **Live QR Image** — QR code rendered as a real scannable image using QR Server API
- 🚫 **Empty Input Validation** — Handles blank input gracefully with a shake animation
- 📱 **Fully Responsive** — Works on mobile, tablet, and desktop
- 🪶 **Zero Dependencies** — No libraries, no npm — pure vanilla JS + external QR API

---

## 🗂️ Project Structure

```
QR-Code-Generator/
│
├── index.html          # Text input, Generate button, QR image container
├── style.css           # Card layout, input/button styling, QR box, animations
├── script.js           # generateQR() — builds API URL, sets image src
├── Logo_Twitter.png    # Twitter/X logo asset
└── twitter-png.png     # Twitter/X icon asset
```

---

## ⚙️ How It Works

```
User types text or URL in the input field
               ↓
Clicks "Generate QR Code" (calls generateQR())
               ↓
JS reads the input value
               ↓
Builds QR Server API URL with the text encoded
               ↓
Sets the <img> src to the API URL
               ↓
Browser fetches & displays the QR code image
               ↓
User can scan the QR code with any phone camera
```

---

## 🌐 QR Code API Used

This project uses the free **QR Server API** to generate QR codes:

```
https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=YOUR_TEXT_HERE
```

| Parameter | Description |
|-----------|-------------|
| `size` | QR code image dimensions (e.g. `150x150`) |
| `data` | The text or URL to encode into the QR |

> 🆓 Completely free — no API key required!

---

## 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| **HTML5** | Input field, image tag, button |
| **CSS3** | Card layout, QR box reveal, shake animation |
| **JavaScript (Vanilla)** | Read input, build API URL, set image src |
| **QR Server API** | Free external API that generates the QR image |
| **Vercel** | Deployment & hosting |

---

## 💡 Key Concepts Demonstrated

- **External API Usage** — Consuming a third-party API via dynamic `<img src>` URL building (no `fetch()` needed!)
- **DOM Manipulation** — Reading input value and updating image element
- **Input Validation** — Preventing empty QR generation with CSS shake animation
- **URL Encoding** — Properly encoding user text into a query string parameter
- **Event Handling** — `onclick` attribute triggering the generator function

---

## 🚀 Getting Started

### Run Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/Daniish-Qureshi/QR-Code-Generator.git
   ```

2. **Navigate into the project folder**
   ```bash
   cd QR-Code-Generator
   ```

3. **Open in browser**
   ```
   Open index.html directly in your browser
   — or use Live Server (VS Code extension)
   ```

> ✅ No API key needed. No npm. No setup. Just open and generate!

---

## 📱 Responsive Design

| Screen | Behavior |
|--------|----------|
| **Mobile** | Full-width centered card, large QR display |
| **Tablet** | Comfortable card width with padding |
| **Desktop** | Centered card with clean spacing |

---

## 🔢 What Can You Encode?

| Input Type | Example |
|------------|---------|
| Plain Text | `Hello World` |
| Website URL | `https://github.com/Daniish-Qureshi` |
| Email | `mailto:email@example.com` |
| Phone Number | `tel:+919999999999` |
| WhatsApp Link | `https://wa.me/919999999999` |
| UPI Payment | `upi://pay?pa=example@upi` |

---

## 👨‍💻 Author

**Danish Qureshi**  
BCA Final Year Student | Full Stack Developer  
📍 Dadri, Uttar Pradesh, India  
🔗 [GitHub — @Daniish-Qureshi](https://github.com/Daniish-Qureshi)  
🌐 [Portfolio](https://danish-qureshi-6ew5.vercel.app)

---

## 📄 License

This project is open source and free to use for **educational & portfolio purposes**.

---

⭐ If you found this useful, give it a **star** on GitHub!
