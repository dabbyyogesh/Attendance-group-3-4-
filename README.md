# 📝 Class Attendance Portal

A lightweight, mobile-first web application designed specifically for Class Representatives (CRs) to efficiently track, manage, and export daily student attendance. 

This project operates entirely in the browser (client-side) and utilizes Firebase for secure, real-time cloud storage. 

## ✨ Features

*   🔒 **Secure Admin Login:** Protected entry ensuring only authorized CRs can access or modify the database.
*   📱 **Mobile-Optimized UI:** Replaced traditional checkboxes with large, color-coded toggle buttons (Present/Absent) for rapid, touch-friendly attendance taking.
*   📅 **Detailed Session Tracking:** Logs attendance using unique identifiers combining **Date**, **Time Slot** (1-hour lectures or 2-hour labs), and **Subject**.
*   📋 **One-Click Reporting:** Automatically generates and copies a clean, formatted text report of present students directly to the clipboard.
*   ☁️ **Cloud Persistence:** Permanent, real-time data storage using Firebase Firestore.
*   ➕ **Dynamic Roster Management:** Secure, password-protected option to add new students to the database on the fly.

## 🛠️ Tech Stack

*   **Frontend:** HTML5, CSS3, Vanilla JavaScript (ES6 Modules)
*   **Backend / Database:** Cloud Firestore (Firebase)
*   **Authentication:** Firebase Auth (Email/Password)
*   **Hosting:** GitHub Pages

## 🔐 Security Note

Because this is a serverless frontend application, the Firebase configuration keys are publicly visible in the source code. **However, the database is completely secure.** 

The database is locked behind strict **Firestore Security Rules** (`request.auth != null`), meaning unauthorized users or scripts cannot read, write, or tamper with the attendance data, even with access to the API keys. 
