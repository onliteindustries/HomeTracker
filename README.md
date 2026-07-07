# 🏠 Home Construction Tracker — Android App

A complete Android phone app to track your home construction:
- Materials used & cost
- Supplier payments (paid / pending)
- Labour / worker payments
- All payment records
- Budget vs spending tracker
- Export to Excel
- Photo / receipt attachment
- Edit & delete records

---

## 📱 How to get the APK on your phone

### Method 1 — GitHub Actions (automatic, recommended)

1. **Create a free GitHub account** at https://github.com
2. **Create a new repository** → name it `HomeTracker` → set to Public
3. **Upload all these files** to the repository (drag & drop in browser)
4. GitHub Actions will **automatically build the APK** — takes ~5 minutes
5. Go to **Actions tab** → click the latest build → scroll down to **Artifacts**
6. Download `HomeTracker-debug-APK`
7. Extract the zip → you get `HomeTracker-debug.apk`
8. **Send the APK to your phone** (WhatsApp, email, USB, Google Drive)
9. On phone: Settings → Install unknown apps → Allow → Open the APK → Install

### Method 2 — Manual build (if you have Android Studio)

```bash
cd android
./gradlew assembleDebug
# APK is at: android/app/build/outputs/apk/debug/app-debug.apk
```

---

## 📁 Project structure

```
HomeTracker/
├── .github/
│   └── workflows/
│       └── build-apk.yml      ← GitHub Actions (auto-builds APK)
├── android/
│   ├── app/
│   │   └── src/main/
│   │       ├── AndroidManifest.xml
│   │       ├── assets/www/
│   │       │   ├── index.html     ← Full app UI
│   │       │   └── xlsx.full.min.js
│   │       ├── java/com/hometracker/
│   │       │   └── MainActivity.java
│   │       └── res/
│   ├── build.gradle
│   ├── settings.gradle
│   └── gradlew
└── README.md
```

---

## ✅ Features

| Feature | Status |
|---|---|
| Materials tracker (qty, rate, total) | ✅ |
| Supplier payments (paid/pending) | ✅ |
| Labour / worker payments | ✅ |
| All payments log with filter | ✅ |
| Project budget & progress bar | ✅ |
| Export to Excel (.xlsx) | ✅ |
| Photo / receipt attachment | ✅ |
| Edit existing records | ✅ |
| Delete with confirmation | ✅ |
| Offline (no internet needed) | ✅ |
| Data saved on phone | ✅ |

---

## 🔧 App details

- **Min Android version**: Android 5.0 (API 21) and above
- **Size**: ~1 MB
- **No internet required** after install
- **Data stored locally** on your phone

---

*Built for Onlite Industries / GVE Brand — Jabalpur*
