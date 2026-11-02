# Mathi Notes

**A clean, fast notes app for Android.** Designed & built by Mathi.

I wanted a notes app that opens instantly, stays out of the way and still does the useful things: reminders, checklists, voice, and turning a printed page into text.

[**⬇ Download Mathi Notes v1.0 (APK, 3.7 MB)**](https://github.com/Mathi-Spartan/Spartan-Speaks---Android-Studio/releases/download/mathi-notes-v1.0/MathiNotes-1.0.apk) · [Install guide](../../docs/INSTALL.md) · [All releases](https://github.com/Mathi-Spartan/Spartan-Speaks---Android-Studio/releases)

<!-- Screenshots: add phone screenshots to apps/mathi-notes/screenshots/ and list them here -->

---

## What it does

### ✍️ Write
- **Notes and checklists:** tick items off as you go, and mark them not done again
- **Pin to top** the notes that matter right now
- **Templates** to start fast: Daily journal, Meeting notes, Packing list, Ideas, Decisions, or a blank page
- **Tags** to keep notes organised (Work, Personal…)

### 👀 Three ways to see your notes
- **Notes:** a clean list grouped by Yesterday, This week and older
- **Cards:** your notes as a grid of cards
- **Board:** columns by tag, like a mini kanban board

### ⏰ Remind
- **Remind me** on any note: today, tomorrow or any time you pick
- Reminders still fire after your phone restarts

### 🎙 Speak
- **Voice notes:** tap the mic, speak, and your words are typed into the note

### 📷 Scan
- **Scan a page:** take a photo of printed text and it becomes an editable note
- Text recognition runs **on your phone** (Google ML Kit). The first scan may take a moment while Google Play services sets up the text model.

### 🔎 Find and keep
- **Search** across all your notes
- **Share** any note to another app
- **Back up** every note to one file you can keep in Google Drive, and **restore** it anytime
- Notes are also included in your phone's own Google backup, so they come back if you reinstall or change phones

---

## Requirements

| | |
|---|---|
| Android | 11 or newer |
| For scanning | A camera app and Google Play services |

## Permissions, and why

| Permission | Why Mathi Notes needs it |
|---|---|
| Notifications | To show your reminders |
| Exact alarms | So reminders ring at exactly the time you set |
| Run at startup | To put your reminders back after the phone restarts |
| Internet / network state | Used by Google's on-device text-recognition component for setup. **Your notes are never uploaded.** |

## Release details

| | |
|---|---|
| Version | 1.0 |
| Package | `com.mathi.notes` |
| Size | 3.7 MB |
| SHA-256 | `3d10afeb446fcd48ec416bbd9866e38f727a5eaf8e566c47c44396eea2927883` |
| Built with | Kotlin + Jetpack Compose, Google ML Kit text recognition |

---

<sub>Designed & built by Mathi, with AI as a pair programmer. [← Back to all apps](../../README.md)</sub>
