# Spartan Speaks: notes for Claude

Mathi's public showcase of his Android apps. Visitors should understand each app and be able to download it.

## Layout
- `README.md`: landing page (banner, app table with download buttons, a closer look, how they're built, privacy).
- `apps/<app>/README.md` + `apps/<app>/screenshots/`: one page per app (features, data flow, requirements, permissions table, release details with SHA-256).
- `docs/INSTALL.md`, `docs/FAQ.md`: for non-technical visitors.
- APKs live in `downloads/` as `<AppName>-<version>.apk`; buttons link to `https://github.com/Mathi-Spartan/Spartan-Speaks---Android-Studio/raw/main/downloads/<file>`. (Claude sessions can't create GitHub Releases; Mathi can switch to Releases himself later.)

## Apps (Nov 2026)
| App | Package | File | Source |
|---|---|---|---|
| Uyir | `dev.mathi.uyir` | `Uyir-1.0.49.apk` | Mathi_TV repo, branch `uyir-health` (CI publishes APK to `uyir-apk`) |
| Mathi Notes | `com.mathi.notes` | `MathiNotes-1.0.apk` | not on GitHub; APK supplied by Mathi |

Parked for later (only add when Mathi says so): Mathi Dust (Mathi_TV `dust-apk`), Thodar, and others.

## Adding an app
1. Get the tested APK; read package/version from its manifest; compute SHA-256.
2. Add `apps/<app>/README.md` (copy an existing one's structure) and screenshots.
3. Add a row to the README table and a section under "A closer look".
4. Add the APK to `downloads/`, remove the old version's file, and check the download link works.
5. Show Mathi a preview before publishing.

## Rules
- Credit: "Designed & built by Mathi", with AI (Claude) as pair programmer.
- Be accurate about privacy and permissions; never claim something the app doesn't do.
- Never commit signing keys or tokens.
