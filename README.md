---

# 🔐 Login Authentication (Local Demo)

A minimal and elegant **login & registration system** built using **HTML, CSS, and vanilla JavaScript**.
This demo securely stores user credentials in the browser using **localStorage + SHA-256 hashing**, making it ideal for learning authentication concepts and UI design.

<svg width="1200" height="350" viewBox="0 0 1200 350" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="grad" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#1e3c72"/>
      <stop offset="50%" stop-color="#2a5298"/>
      <stop offset="100%" stop-color="#7e22ce"/>
    </linearGradient>
  </defs>

  <rect width="1200" height="350" fill="url(#grad)" rx="20" />

  <!-- lock icon -->
  <g transform="translate(120, 95) scale(3.2)" fill="white" opacity="0.9">
    <path d="M17 8V6a6 6 0 1 1 12 0v2h3a2 2 0 0 1 2 2v18a2 2 0 0 1-2 2H14a2 2 0 0 1-2-2V10a2 2 0 0 1 2-2h3zm2 0h10V6a4 4 0 1 0-10 0v2zm5 12a3 3 0 1 0 0-6 3 3 0 0 0 0 6z"/>
  </g>

  <!-- Title -->
  <text x="430" y="180" fill="white" font-size="54" font-weight="700" font-family="Segoe UI, sans-serif">
    Login Authentication System
  </text>

  <!-- subtitle -->
  <text x="430" y="235" fill="#e5e7eb" font-size="26" font-family="Segoe UI, sans-serif">
    HTML • CSS • JavaScript • LocalStorage • SHA-256
  </text>
</svg>


---

## ⭐ Features

* Clean and modern UI built with pure CSS
* Create Account + Sign In flow
* SHA-256 password hashing (no plaintext storage)
* LocalStorage-based account persistence
* Error handling and form validation
* Protected “Signed-In Area” view
* Ability to delete account
* Fully responsive design

---

## 📁 Project Structure

```
project/
│── index.html
│── README.md
└── assets/
    └── banner.png
```

---

## 🚀 Live Demo (Local)

Run using any local server:

```bash
python -m http.server
```

Then open:

```
http://localhost:8000
```

---

## 🧠 How It Works

### 🔸 Registration

* User enters username, email, password
* Password is hashed using **SHA-256**
* Data is stored in localStorage as:

```
{ username: { email, hash, createdAt } }
```

### 🔸 Login

* User enters username + password
* Hash is compared with stored value
* On success, user enters a protected area

### 🔸 Protected View

Displays:

* Username
* Account creation date
* Sign out & Delete account options

---

## 🛠 Technologies Used

| Technology                 | Purpose              |
| -------------------------- | -------------------- |
| **HTML5**                  | Structure            |
| **CSS3**                   | Styling (Custom UI)  |
| **JavaScript (Vanilla)**   | Authentication logic |
| **LocalStorage**           | Data persistence     |
| **SHA-256 Web Crypto API** | Secure hashing       |

---

## 📷 Screenshots

### Login UI

![login](https://dummyimage.com/900x500/f3f4f6/111\&text=Login+Screen)

### Create Account

![register](https://dummyimage.com/900x500/f3f4f6/111\&text=Register+Screen)

### Signed-In Dashboard

![dashboard](https://dummyimage.com/900x500/f3f4f6/111\&text=Signed+In)

---

## ⚠️ Important Note

This authentication is **for learning purposes only**.
It should **NOT** be used in real applications because:

* LocalStorage is not secure
* No backend or database
* No session tokens

---

## 📄 License

MIT License. Free to use, learn, and modify.

---

## 🙌 Author

Built by **Vedansh Harish Ail**.

---

If you want:
✅ A matching banner (PNG or SVG)
✅ Dark theme version of README
✅ GitHub badges section
Just tell me: **"Add badges"** or **"Give dark theme README"**
