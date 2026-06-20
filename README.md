# 🏏 CricScore Premium - Live Cricket Tournament Scorer

CricScore Premium is a modern, real-time cricket match scoring and tournament management web application. It allows local umpires to digitally score matches from the ground while broadcasting the live score to viewers anywhere in the world without requiring page refreshes.

## 🌟 Key Features
* **🔴 Real-Time Live Sync:** Powered by Firebase Realtime Database. Scores update on viewers' screens instantly.
* **📱 Premium Responsive UI:** Mobile-first design that looks and feels like a professional top-tier cricket app.
* **🔒 Secure Admin Panel:** Protected by a secret PIN to prevent unauthorized score tampering.
* **👥 Team Management:** Create and manage local teams directly from the dashboard.
* **📊 Match Setup:** Select batting/bowling teams and customize match overs (2, 5, 10, or 20 overs).
* **🏏 Advanced Keypad:** Easy one-tap scoring for Runs, Wickets, Wides, and No-Balls (with run tracking).
* **↩️ Undo Feature:** Made a mistake? Quickly undo the last ball bowled.
* **📜 Match History:** Automatically saves completed match results with date, teams, and final scores.

## 📂 Project Structure
The project is split into two lightweight, secure files:
1.  `index.html` - **Public View:** Only displays the live score. No buttons, no scoring capabilities. Share this link with viewers.
2.  `admin.html` - **Umpire/Admin View:** The locked control panel for the scorer. Requires a PIN to access the keypad and setup options.

## 🛠️ Technology Stack
* **Frontend:** HTML5, CSS3 (Custom Variables & Gradients), Vanilla JavaScript
* **Backend/Database:** Google Firebase Realtime Database
* **Hosting Recommendation:** Netlify (Free & easy drag-and-drop deployment)

## 🚀 Setup & Installation Guide

### Step 1: Firebase Setup
1. Create a free account on [Firebase Console](https://console.firebase.google.com/).
2. Create a new project and add a "Web App".
3. Create a **Realtime Database** and start it in **Test Mode** (so the app can read/write data).
4. Copy your `firebaseConfig` object provided by Firebase.

### Step 2: Code Configuration
1. Open both `index.html` and `admin.html` in a text editor.
2. Locate the `firebaseConfig` section in the `<script>` tag.
3. Replace the placeholder values with your actual Firebase API keys.

### Step 3: Admin PIN Setup
1. Open `admin.html`.
2. Locate the line: `const SECRET_PIN = "12345";`
3. Change `"12345"` to your desired secure password.

### Step 4: Hosting (Making it Live)
1. Go to [Netlify Drop](https://app.netlify.com/drop).
2. Drag and drop your project folder (containing both HTML files).
3. Netlify will generate a live link (e.g., `https://your-tournament.netlify.app`).
4. **Share with public:** Give them the main link (`/index.html`).
5. **For Umpire:** Add `/admin.html` to the link (e.g., `https://your-tournament.netlify.app/admin.html`).

## 👨‍💻 Author
Developed and Designed by **LEGEND KILLER**.

---
*Note: This is a client-side web application. Clear your browser cache if you want to completely wipe the locally saved teams and match history.*
