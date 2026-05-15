# Mahila-Shakti Unnati – Digital SHG Management App

![Android](https://img.shields.io/badge/Platform-Android-green)
![Kotlin](https://img.shields.io/badge/Language-Kotlin-blue)
![Jetpack Compose](https://img.shields.io/badge/UI-Jetpack%20Compose-orange)
![Room DB](https://img.shields.io/badge/Database-RoomDB-red)
![MVVM](https://img.shields.io/badge/Architecture-MVVM-purple)

## 📌 Overview

**Mahila-Shakti Unnati** is a GenAI-powered Android application developed for Women Self-Help Groups (SHGs) to digitally manage savings, loans, and member records.

The app replaces traditional paper-based bookkeeping with a secure and offline-first digital ledger system. It acts as a **Digital Accountant** that improves transparency, reduces manual errors, and simplifies financial management for SHGs.

---

# ✨ Features

## 👥 Member Management
- Add, edit, and delete SHG members
- Store member details:
  - Name
  - Phone Number
  - Photo
  - Unique Member ID

## 💰 Savings Tracking
- Weekly savings entry system
- Mark contributions as:
  - Paid
  - Pending
- Real-time savings total updates

## 🏦 Loan Management
- Issue loans to members
- Prevent multiple unpaid loans
- Track:
  - Principal amount
  - Interest
  - Repayment history

## 🤖 GenAI Financial Q&A
Ask questions in natural language such as:
- “How much has Rani saved?”
- “Who has pending loans?”
- “Show total group capital”

Uses Gemini AI with local database context for accurate responses.

## 📤 WhatsApp Export
- Generate monthly summaries
- Share reports using Android Share Intent

## 📶 Offline First
- Works without internet
- Uses Room Database for local storage

---

# 🏗️ Tech Stack

| Technology | Purpose |
|---|---|
| Kotlin | Android Development |
| Jetpack Compose | UI Development |
| MVVM Architecture | Clean Architecture |
| Room Database | Offline Local Storage |
| Repository Pattern | Data Layer |
| SQLCipher | Database Encryption |
| Gemini AI | AI-powered Q&A |

---

# 🧠 Architecture

The project follows the **MVVM (Model-View-ViewModel)** architecture pattern.

```text
UI (Compose Screens)
        ↓
ViewModel
        ↓
Repository
        ↓
Room Database
```

---

# 📂 Project Structure

```text
app/
│
├── data/
│   ├── local/
│   ├── repository/
│   └── model/
│
├── ui/
│   ├── screens/
│   ├── components/
│   └── theme/
│
├── viewmodel/
│
├── utils/
│
└── MainActivity.kt
```

---

# ⚙️ Business Logic

## Simple Interest Formula

```text
SI = (P × R × T) / 100
```

Where:
- **P** = Principal Amount
- **R** = Rate of Interest
- **T** = Time

## Loan Eligibility Rule

A member cannot receive a new loan if:
- Existing loan is unpaid
- Outstanding balance is greater than zero

---

# 🔒 Security Features

- Local PIN authentication
- Encrypted Room Database using SQLCipher
- Offline data protection

---

# 🌍 Accessibility Features

- Hindi & English support
- Large touch-friendly UI
- Simple interface for rural users

---

# 🚀 Installation

## Prerequisites

- Android Studio
- Kotlin
- Android SDK
- Minimum SDK 24+

## Clone Repository

```bash
git clone https://github.com/ttv26/mahila-shakti-unnati.git
```

## Open in Android Studio

1. Open Android Studio
2. Select **Open Project**
3. Choose the cloned project folder
4. Sync Gradle files

## Run the App

- Connect Android device or emulator
- Click ▶ Run

---

# 📊 Success Criteria

- Real-time dashboard updates
- Offline functionality
- Accurate AI responses
- Loan conflict prevention
- Easy report sharing

---

# 🔮 Future Enhancements

- Cloud synchronization
- Biometric authentication
- NGO/Bank dashboard
- Multi-device sync
- Analytics dashboard

---

# 📸 Screenshots

<img width="1080" height="2400" alt="Screenshot_2026-05-11-21-57-30-711_com example unnati" src="https://github.com/user-attachments/assets/ec39a462-b8ac-45d2-bdcb-1bb49998d8dc" />
<img width="1080" height="2400" alt="Screenshot_2026-05-11-21-56-56-295_com example unnati" src="https://github.com/user-attachments/assets/73cdf149-e757-42a4-b73c-ef449c9845f4" />
<img width="1080" height="2400" alt="Screenshot_2026-05-11-21-55-02-469_com example unnati" src="https://github.com/user-attachments/assets/0b9a28ed-717e-42fd-bb52-ce11256e0b20" />
<img width="1080" height="2400" alt="1778516431106" src="https://github.com/user-attachments/assets/db0abb77-e4d8-4703-a3a3-d4995625b81d" />


```text
screenshots/
├── dashboard.png
├── members.png
├── loans.png
└── reports.png
```

---

# 📄 License

This project is licensed under the MIT License.
