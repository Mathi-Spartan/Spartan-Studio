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
| Kurippu (குறிப்பு), formerly Mathi Notes | `com.mathi.notes` | `Kurippu-1.0.apk` | not on GitHub; APK supplied by Mathi. The v1.0 APK still shows the label "Mathi Notes"; a rebuild should rename it to Kurippu, keeping the package name and signing key so it updates in place |

Parked for later (only add when Mathi says so): Mathi Dust (Spartan_TV_Apps branch `launchers`, `mathi-dust/release/`), Thodar, and others.

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
