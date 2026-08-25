# Study App — Changelog

## Step 1 — Project shell + CI build pipeline (current)
Starting point. No study features yet — this just proves the build pipeline works end-to-end.

**Added:**
- Basic Android app skeleton (Kotlin, single `MainActivity`)
- Placeholder home screen showing the app is alive
- `.github/workflows/build.yml` — GitHub Actions workflow that builds a debug APK automatically on every push to `main`, downloadable from the Actions tab as an artifact (`study-app-debug`)
- Project configured with: compileSdk 34, minSdk 26, targetSdk 34, Kotlin 1.9.24, AGP 8.5.2, Gradle 8.7

**Not yet implemented:**
- App-selector + blocking during study sessions
- Alarm-style study reminders
- Away-from-phone tracking (excluding 12am–6:30am sleep window)
- Rewards engine, graphs, redemption for game/call time

---

## Planned next: Step 2 — App blocker
- Pick which apps get restricted during a study session
- Detect and force-close/block those apps for the session duration
