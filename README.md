<p align="center">
  <img src="assets/banner.svg" alt="Spartan Studio: Android apps designed and built by Mathi" width="100%">
</p>

<p align="center">
  <b>A home for the Android apps I design for my own phone and share with everyone.</b><br>
  Each one started as an idea, went through design mockups, and was built with an AI pair programmer.
</p>

<p align="center">
  <a href="#-the-apps">The apps</a> ·
  <a href="docs/INSTALL.md">How to install</a> ·
  <a href="#-how-these-apps-are-built">How they're built</a> ·
  <a href="docs/FAQ.md">FAQ</a>
</p>

---

## 📱 The apps

| | App | What it does | Download |
|:--:|---|---|:--:|
| <img src="apps/uyir/screenshots/today.jpg" width="110"> | **[Uyir (உயிர்)](apps/uyir/README.md)**<br><sub>Health · v1.0.49 · 10 MB · Android 9+</sub> | Your own health dashboard for the **Fitbit Air**. Recovery, sleep and strain scores, sleep stages, trends and a private journal that shows what actually moves your HRV. | [**⬇ Download APK**](https://github.com/Mathi-Spartan/Spartan-Studio/raw/main/downloads/Uyir-1.0.49.apk) |
| <img src="apps/kurippu/screenshots/list.jpg" width="110"> | **[Kurippu (குறிப்பு)](apps/kurippu/README.md)**<br><sub>Productivity · v1.0 · 3.7 MB · Android 11+</sub> | A clean, fast notes app. Checklists, reminders, voice notes, and **scan a printed page straight into a note**. | [**⬇ Download APK**](https://github.com/Mathi-Spartan/Spartan-Studio/raw/main/downloads/Kurippu-1.0.apk) |
| <img src="apps/suvadi/screenshots/home.jpg" width="110"> | **[Suvadi (சுவடி)](apps/suvadi/README.md)**<br><sub>Books · v1.0.51 · 2.9 MB · Android 8+</sub> | A modern **Tamil library**: 1,281 books from Project Madurai, Thanglish search, an offline reader with **Tamil read-aloud**, a literary map, and a Kural of the day widget. | [**⬇ Download APK**](https://github.com/Mathi-Spartan/Spartan-Studio/raw/main/downloads/Suvadi-1.0.51.apk) |

> **New to installing apps from outside the Play Store?** It takes about a minute. Follow the [step-by-step install guide](docs/INSTALL.md).

All APK files are in the [downloads folder](downloads/), and each app's page lists a checksum so you can verify your file.

---

## ✨ A closer look

### Uyir (உயிர்), your health, your way

*Uyir* means "life" in Tamil. I bought a Fitbit Air and didn't enjoy the stock app, so I designed my own.

<p>
  <img src="apps/uyir/screenshots/today.jpg" width="200" alt="Uyir home screen">
  <img src="apps/uyir/screenshots/sleep.jpg" width="200" alt="Uyir sleep screen">
  <img src="apps/uyir/screenshots/trends.jpg" width="200" alt="Uyir trends screen">
  <img src="apps/uyir/screenshots/journal.jpg" width="200" alt="Uyir journal screen">
</p>

- **Daily scores:** Recovery, Strain and Sleep, calculated by Uyir on your phone
- **Sleep in detail:** a stage-by-stage timeline, sleep score, bedtime consistency and sleep goals
- **Trends:** HRV, resting heart rate, steps and weight over weeks
- **Journal:** tag your evenings (alcohol, late workout, screens in bed…) and Uyir shows which habits raise or lower your HRV
- **Your photo** on the home card, **CSV export**, and a **sample-data mode** so you can explore without a watch

[Full details →](apps/uyir/README.md)

### Kurippu (குறிப்பு), notes without the clutter

*Kurippu* means "a note" in Tamil.

<p>
  <img src="apps/kurippu/screenshots/list.jpg" width="200" alt="Kurippu notes list">
  <img src="apps/kurippu/screenshots/board.jpg" width="200" alt="Kurippu board view">
  <img src="apps/kurippu/screenshots/new.jpg" width="200" alt="Create a new note">
  <img src="apps/kurippu/screenshots/backup.jpg" width="200" alt="Backup and restore">
</p>

- **Notes and checklists**, pinned to the top when they matter
- **Three views:** a clean list, cards, or a board with a column for each tag
- **Reminders** that ring on time and survive a phone restart
- **Voice notes:** speak and it types for you
- **Scan a page:** point the camera at printed text and it becomes an editable note, read on the phone
- **Templates** for a daily journal, meeting notes, a packing list and more
- **Search, share, back up and restore**

[Full details →](apps/kurippu/README.md)

### Suvadi (சுவடி), the Tamil library in your pocket

*Suvadi* means a palm-leaf manuscript. It is 1,281 Tamil books, from the Sangam poems and Thirukkural to Bharathiyar and Kalki, in one reader.

<p>
  <img src="apps/suvadi/screenshots/home.jpg" width="200" alt="Suvadi home">
  <img src="apps/suvadi/screenshots/library.jpg" width="200" alt="Suvadi library">
  <img src="apps/suvadi/screenshots/reader.jpg" width="200" alt="Suvadi reader">
  <img src="apps/suvadi/screenshots/map.jpg" width="200" alt="Literary map of Tamil Nadu">
</p>

- **Search in Tamil, English or Thanglish:** `kural` finds திருக்குறள்
- **Read inside the app** in day, sepia or night themes, and **listen in Tamil**
- **Offline:** every book you open stays on your phone
- **Highlight** and **share any verse as an image**
- **Explore:** a journey through 7 eras, a literary map of Tamil Nadu, and the Palayakkarar Resistance in Tamil and English
- **Streaks, badges**, and a **Kural of the day** home-screen widget

[Full details →](apps/suvadi/README.md)

---

## 🤖 How these apps are built

I'm a developer, and these apps are built **with AI as my pair programmer** ([Claude](https://claude.ai) by Anthropic). The ideas, the design calls and the testing are mine. The AI helps me move from idea to working app much faster than I could alone.

Every app follows the same path:

```
💡 Idea → 🎨 Mockups → ✅ Approve → 🛠 Build → 📱 Daily use → 🚀 Release
```

1. **Idea:** a real problem from my own day (a health app I didn't like, notes that felt cluttered).
2. **Mockups:** interactive design prototypes, often several rounds, until it feels right.
3. **Approval:** nothing gets built until I'm happy with how it looks.
4. **Build:** native Android apps (Kotlin, Jetpack Compose or a WebView-based UI), compiled and signed into an APK.
5. **Real-world testing:** I use every app on my own phone before it's published here.
6. **Release:** the tested APK is published here for anyone to download.

---

## 🔒 Privacy promise

- **No accounts, no ads, no tracking.**
- Your notes and your health data **stay on your phone**. These apps have no servers.
- Every app's page lists exactly which permissions it asks for, and why.

---

## 🗺 What's next

More apps are on the way, and each will be added here once it has passed daily use on my own phone. Watch or star this repo to hear about new releases.

---

<p align="center">
  Designed &amp; built by <b>Mathi</b> · <a href="https://github.com/Mathi-Spartan">@Mathi-Spartan</a><br>
  <sub>Found a bug or have an idea? <a href="https://github.com/Mathi-Spartan/Spartan-Studio/issues">Open an issue</a>.</sub>
</p>
