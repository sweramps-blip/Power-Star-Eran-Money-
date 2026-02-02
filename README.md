# 🌟 POWER STAR EARNING PLATFORM

> **Professional Social Media Task & Referral Earning Platform**

![Status](https://img.shields.io/badge/Status-Ready%20to%20Deploy-success)
![Version](https://img.shields.io/badge/Version-1.0.0-blue)
![License](https://img.shields.io/badge/License-Proprietary-red)

---

## 📋 TABLE OF CONTENTS

1. [Overview](#overview)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Project Structure](#project-structure)
5. [Installation](#installation)
6. [Configuration](#configuration)
7. [Usage](#usage)
8. [API Documentation](#api-documentation)
9. [Database Schema](#database-schema)
10. [Troubleshooting](#troubleshooting)

---

## 🎯 OVERVIEW

Power Star is a complete earning platform where users can:
- **Complete social media tasks** (YouTube, Facebook, Instagram, TikTok, LinkedIn)
- **Earn through referrals** (5% lifetime commission + Rs. 50 join bonus)
- **Market digital products**
- **Withdraw earnings** via Easypaisa/JazzCash

### Key Statistics:
- **Tech:** Pure HTML/CSS/JavaScript (No framework required)
- **Backend:** Google Apps Script (Free & Scalable)
- **Database:** Google Sheets (Real-time sync)
- **Hosting:** Compatible with any static hosting (GitHub Pages, Netlify, etc.)

---

## ✨ FEATURES

### User Features:
- ✅ **Secure Registration** with device lock
- ✅ **Login System** with password protection
- ✅ **Dashboard** with real-time balance
- ✅ **Task System** with daily limits
- ✅ **Referral Program** (5% lifetime + Rs. 50 bonus)
- ✅ **Wallet Management** (Bind Easypaisa/JazzCash)
- ✅ **Withdrawal System** (Min: Rs. 525, Max: Rs. 50,000)
- ✅ **Transaction History**
- ✅ **Announcements** (Text & Image support)

### Admin Features:
- 🔐 **Secure Admin Panel** (Password protected)
- 👥 **User Management** (Search by PSSN ID)
- 💰 **Send Money** (Salary/Reward/Bonus)
- ✅ **Withdrawal Approval System**
- 📊 **Task Management**
- 📢 **Announcement System**

---

## 🛠 TECH STACK

### Frontend:
- **HTML5** - Structure
- **CSS3** - Styling (Modern gradient designs)
- **JavaScript (ES6+)** - Logic & API calls
- **SweetAlert2** - Beautiful alerts
- **Font Awesome** - Icons
- **Google Fonts** - Typography (Poppins, Outfit)

### Backend:
- **Google Apps Script** - Server-side logic
- **Google Sheets** - Database

### External Services:
- **Image Hosting** - Imgur/ImgBB (for screenshots)
- **Payment Integration** - Manual (Easypaisa/JazzCash)

---

## 📁 PROJECT STRUCTURE

```
Power-Star-Eran-Money/
│
├── index.html              # Landing page
├── auth.html               # Login/Registration
├── dashboard.html          # User dashboard
├── marketing.html          # Tasks & Products ⭐ NEW
├── team.html               # Referral management
├── wallet.html             # Withdrawal & binding
├── history.html            # Transaction history
├── admin_power_786.html    # Admin panel
│
├── config.js               # Unified configuration ⭐ NEW
├── APPS_SCRIPT.gs          # Backend code ⭐ NEW
│
├── docs/
│   ├── PROJECT_REVIEW_URDU.md      # Complete review (Urdu)
│   ├── SETUP_GUIDE_URDU.md         # Installation guide (Urdu)
│   ├── DATABASE_STRUCTURE.md       # Database schema
│   └── README.md                   # This file
│
└── assets/                 # (Optional) Images/icons
```

---

## 🚀 INSTALLATION

### Prerequisites:
- Google account
- Text editor (VS Code recommended)
- Web browser
- Basic understanding of HTML/JavaScript

### Step 1: Clone Repository
```bash
git clone https://github.com/yourusername/Power-Star-Eran-Money.git
cd Power-Star-Eran-Money
```

### Step 2: Setup Google Sheet
1. Create new Google Sheet: [sheets.google.com](**
3. Create these tabs:
   - USERS_MASTER
   - WITHDRAWALS
   - ACCOUNT_BINDINGS
   - TRANSACTIONS
   - ANNOUNCEMENTS
   - TASKS
   - TASK_SUBMISSIONS

4. Add headers (see [DATABASE_STRUCTURE.md](docs/DATABASE_STRUCTURE.md))

### Step 3: Deploy Apps Script
1. Open Sheet → **Extensions** → **Apps Script**
2. Delete default code
3. Copy code from `APPS_SCRIPT.gs`
4. **Save** → **Deploy** → **New Deployment**
5. Type: **Web app**
6. Execute as: **Me**
7. Who has access: **Anyone**
8. Click **Deploy**
9. **Copy the deployment URL**

### Step 4: Configure Project
1. Open `config.js`
2. Replace `YOUR_SCRIPT_ID_HERE` with your deployment URL
3. Update admin numbers if needed
4. Change admin password (recommended)

### Step 5: Deploy Website
Choose one:

**Option A: GitHub Pages (Recommended)**
```bash
git add .
git commit -m "Initial commit"
git push origin main
# Go to repo Settings → Pages → Enable
```

**Option B: Netlify**
1. Drag & drop folder to [netlify.com/drop](https://netlify.com/drop)
2. Get instant URL

**Option C: Local Testing**
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx http-server
```

---

## ⚙️ CONFIGURATION

### config.js Settings:

```javascript
const POWER_STAR_CONFIG = {
    // 🔴 CRITICAL: Replace with your Apps Script URL
    API_URL: "https://script.google.com/macros/s/.../exec",
    
     
    
    
    
    // Financial settings
    MIN_WITHDRAWAL: 525,
    MAX_WITHDRAWAL: 50000,
    WITHDRAWAL_FEE: 0.05,    // 5%
    JOIN_BONUS: 50,
    COMMISSION_RATE: 0.05    // 5%
};
```

### Security Checklist:
- [ ] Change `SECURITY_KEY`
- [ ] Update `ADMIN_PASSWORD`
- [ ] Add your admin number
- [ ] Don't share Apps Script URL publicly
- [ ] Enable 2FA on Google account

---

## 📖 USAGE

### For Users:

1. **Registration:**
   - Visit website → Click "Start Earning Now"
   - Fill: Name, Phone (+92), Password
   - Optional: Referral code
   - Accept terms → Register

2. **Login:**
   - Enter phone number & password
   - Dashboard will load

3. **Complete Tasks:**
   - Go to Marketing tab
   - Choose platform (YouTube, Facebook, etc.)
   - Click "Start Task"
   - Complete the task
   - Submit screenshot
   - Wait for approval

4. **Build Team:**
   - Go to Team tab
   - Copy your referral link
   - Share on WhatsApp/Telegram
   - Earn Rs. 50 per member + 5% commission

5. **Withdraw Money:**
   - Go to Wallet tab
   - Bind Easypaisa/JazzCash account (one-time)
   - Enter withdrawal amount
   - Submit request
   - Receive within 24 hours

### For Admins:

1. **Access Admin Panel:**
   - Login with admin number
   - Click "ADMIN PANEL" button
   - Enter password: `Hussain@2025`

2. **Manage Users:**
   - Search by PSSN ID
   - View balance & commission
   - Send Salary/Reward/Bonus

3. **Approve Withdrawals:**
   - View pending requests
   - Check account details
   - Click "Approve Payment"

4. **Create Tasks:**
   - Go to TASKS sheet
   - Add new row with task details
   - Set status to "active"

5. **Post Announcements:**
   - Go to ANNOUNCEMENTS sheet
   - Add message & image URL
   - Set status to "active"
   - Old announcements auto-deactivate

---

## 🔌 API DOCUMENTATION

### GET Endpoints:

```javascript
// Get all users
GET /exec?action=getAllUsers
Response: Array of user objects

// Get specific user
GET /exec?action=getUser&number=3001234567
Response: User object

// Get active tasks
GET /exec?action=getTasks
Response: Array of task objects

// Get announcement
GET /exec?action=getAnnouncement
Response: Announcement object
```

### POST Actions:

```javascript
// Register user
POST /exec
Body: {
    key: "SECURITY_KEY",
    action: "REGISTER",
    name: "Ali Khan",
    number: "3001234567",
    password: "pass123",
    referral: "PSSN0001"
}

// Bind account
POST /exec
Body: {
    key: "SECURITY_KEY",
    action: "BINDING",
    number: "3001234567",
    wallet_name: "Easypaisa",
    acc_number: "03001234567",
    acc_title: "Ali Khan"
}

// Create withdrawal
POST /exec
Body: {
    key: "SECURITY_KEY",
    action: "WITHDRAWAL",
    number: "3001234567",
    w_amount: 1000
}

// Submit task
POST /exec
Body: {
    key: "SECURITY_KEY",
    action: "SUBMIT_TASK",
    number: "3001234567",
    user_id: "PSSN0001",
    task_id: "TASK0001",
    screenshot_url: "https://..."
}

// Admin: Send money
POST /exec
Body: {
    key: "SECURITY_KEY",
    action: "SALARY", // or REWARD, BONUS
    number: "3001234567",
    w_amount: 500,
    target_field: "balance"
}
```

---

## 💾 DATABASE SCHEMA

### Main Tables:

**USERS_MASTER:**
- Primary user data
- Balance tracking
- Referral information
- Device security

**WITHDRAWALS:**
- Withdrawal requests
- Status tracking (pending/success)
- Payment details

**ACCOUNT_BINDINGS:**
- Easypaisa/JazzCash accounts
- One-to-one with users

**TRANSACTIONS:**
- Complete audit log
- All financial movements
- Balance history

**TASKS:**
- Available earning tasks
- Platform-specific
- Daily limits

**TASK_SUBMISSIONS:**
- User task submissions
- Screenshot proofs
- Approval tracking

See [DATABASE_STRUCTURE.md](docs/DATABASE_STRUCTURE.md) for complete schema.

---

## 🐛 TROUBLESHOOTING

### Common Issues:

**1. "Unauthorized" Error**
- Check API URL in config.js
- Verify SECURITY_KEY matches
- Redeploy Apps Script

**2. Data Not Saving**
- Check Apps Script permissions
- Verify sheet tab names
- Check column headers

**3. Commission Not Calculating**
- Check referral code format
- Verify team.html API calls
- Check USERS_MASTER.referral column

**4. Withdrawal Fails**
- Verify account binding first
- Check minimum balance (Rs. 525)
- Ensure sufficient balance

**5. Tasks Not Showing**
- Add tasks to TASKS sheet
- Set status = "active"
- Check API URL in marketing.html

### Debug Mode:
```javascript
// Add to console
localStorage.setItem('debug', 'true');

// View API responses
console.log('User:', PSConfig.getUser());
```

---

## 📞 SUPPORT

**Documentation:**
- [Urdu Setup Guide](docs/SETUP_GUIDE_URDU.md)
- [Database Structure](docs/DATABASE_STRUCTURE.md)
- [Project Review (Urdu)](docs/PROJECT_REVIEW_URDU.md)

**Contact:**
- WhatsApp: +92 XXX XXXXXXX
- Telegram: @PowerStarSupport
- Email: support@powerstar.com

---

## 📄 LICENSE

This project is proprietary software. All rights reserved.

Unauthorized copying, distribution, or modification is prohibited.

---

## 🙏 CREDITS

**Developer:** Power Star Team
**Framework:** Google Apps Script
**Design:** Modern Gradient UI
**Icons:** Font Awesome
**Fonts:** Google Fonts (Poppins, Outfit)

---

## 🚀 ROADMAP

### Version 1.1 (Planned):
- [ ] Email notifications
- [ ] OTP verification
- [ ] Multi-level referral (3 levels)
- [ ] Mobile app (React Native)

### Version 2.0 (Future):
- [ ] Payment gateway integration
- [ ] Automated withdrawals
- [ ] Real-time dashboard
- [ ] Analytics & reports
- [ ] Multi-language support

---

## 📊 STATISTICS

- **Files:** 8 HTML pages
- **Backend:** 1 Apps Script (~500 lines)
- **Database:** 7 sheets
- **Features:** 15+ core features
- **Design:** Fully responsive
- **Security:** Device lock + encryption

---

**Made with ❤️ in Pakistan**

**اللہ آپ کو کامیابی دے**

---

## URDU VERSION (اردو میں)

### تعارف:

پاور اسٹار ایک مکمل کمائی کا پلیٹ فارم ہے جہاں آپ:
- سوشل میڈیا ٹاسک مکمل کر کے کماتے ہیں
- ریفرل سے کمیشن کماتے ہیں (5% لائف ٹائم)
- ڈیجیٹل پروڈکٹس کی مارکیٹنگ کرتے ہیں
- ای ذی پیسہ/جاز کیش سے رقم نکالتے ہیں

### خصوصیات:
✅ محفوظ رجسٹریشن
✅ ڈیوائس لاک
✅ ٹاسک سسٹم
✅ ریفرل پروگرام (رپے 50 + 5%)
✅ واپسی کا نظام

### انسٹالیشن:
مکمل اردو گائیڈ کے لیے دیکھیں: [SETUP_GUIDE_URDU.md](docs/SETUP_GUIDE_URDU.md)

---

**الحمدللہ - پروجیکٹ مکمل!** ✅

