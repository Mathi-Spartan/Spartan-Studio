# Spartan Studio: project notes (repo Mathi-Spartan/Spartan-Studio, formerly Spartan-Speaks---Android-Studio)

Mathi's public showcase of his Android apps. Visitors should understand each app and be able to download it.

## Layout
- `README.md`: landing page (banner, app table with download buttons, a closer look, how they're built, privacy).
- `apps/<app>/README.md` + `apps/<app>/screenshots/`: one page per app (features, data flow, requirements, permissions table, release details with SHA-256).
- `docs/INSTALL.md`, `docs/FAQ.md`: for non-technical visitors.
- APKs live in `downloads/` as `<AppName>-<version>.apk`; buttons link to `https://github.com/Mathi-Spartan/Spartan-Studio/raw/main/downloads/<file>`. (Automated sessions can't create GitHub Releases; Mathi can switch to Releases himself later.)

## Apps (Nov 2026)
| App | Package | File | Source |
|---|---|---|---|
| Uyir | `dev.mathi.uyir` | `Uyir-1.0.49.apk` | Spartan_TV_Apps repo (private), branch `phone-apps`, folder `uyir/` (CI builds the APK into `uyir/release/`) |
| Suvadi (சுவடி) | `dev.mathi.suvadi` | `Suvadi-1.0.51.apk` | Spartan_TV_Apps repo (private), branch `phone-apps`, folder `suvadi/` (CI builds the APK into `suvadi/release/`); data copied from the Suvadi website (Spartan_Web_Apps, branch `personal-projects`, folder `suvadi/`) |
| Kurippu (குறிப்பு), formerly Mathi Notes | `dev.mathi.kurippu` | `Kurippu-1.1.1.apk` | Spartan_TV_Apps repo (private), branch `phone-apps`, folder `kurippu/` (CI builds `kurippu/release/Kurippu.apk` and the Play bundle `Kurippu.aab`). Rebuilt from scratch in Nov 2026 because the old source was lost; the old v1.0 (`com.mathi.notes`) is a different app ID, so it installs side by side and notes move over with Back up / Restore |

Parked for later (only add when Mathi says so): Mathi Dust (Spartan_TV_Apps branch `launchers`, `mathi-dust/release/`), Thodar, and others.

## The rule: "Android - 2026"
Every new Android app request starts with the keyword **Android - 2026**. The app is built in the private Mathi-Spartan/Spartan_TV_Apps repo first (phone apps on branch `phone-apps`). It comes here **only after Mathi has tested it on his phone and confirmed it**. Each time, update the READMEs in both repos: here the app table, the app's page and this file; in Spartan_TV_Apps the app's "Also published in" column.

## Adding an app
All code and signing keys live in the private Mathi-Spartan/Spartan_TV_Apps repo. Copy only the APK, README and screenshots here, never `signing/` or workflows; run `bash tools/check-public-safe.sh <folder>` from Spartan_TV_Apps (`main`) first. See SIGNING.md there.

1. Get the tested APK; read package/version from its manifest; compute SHA-256.
2. Add `apps/<app>/README.md` (copy an existing one's structure) and screenshots.
3. Add a row to the README table and a section under "A closer look".
4. Add the APK to `downloads/`, remove the old version's file, and check the download link works.
5. Show Mathi a preview before publishing.

## Rules
- Commits: author and committer `Mathi-Spartan <291456388+Mathi-Spartan@users.noreply.github.com>`. Never add co-author or AI attribution lines to commits; Mathi must be the only contributor.
- Credit: "Designed & built by Mathi", with an AI pair programmer.
- Be accurate about privacy and permissions; never claim something the app doesn't do.
- Never commit signing keys or tokens.
