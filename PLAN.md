# Quiet TV: Rename from Free My TV

## Overview
This project is being renamed from "Free My TV" to "Quiet TV". This plan covers all phases of the rename.

## Phase 1: Rename (pending)
- Rename the app everywhere to Quiet TV:
  - App package: `io.quiettv` → `io.quiettv`
  - App title: "Free My TV" → "Quiet TV"
  - Build output: `QuietTV.apk` → `QuietTV.apk`
  - LG webOS: `QuietTV-webos.ipk` → `QuietTV-webos.ipk`
  - Samsung Tizen: `QuietTV-tizen.wgt` → `QuietTV-tizen.wgt`
  - Git repo: simbasjungles/quiettv → new repo (heyitsyajat)
  - README: all references updated
  - docs/: all references to freemytv.io updated
  - Credits/license: keep original attribution
  - Keep "Free My TV" only in credits and attribution section

### Files to rename/modify:
- `app/AndroidManifest.xml` - package, label, theme names
- `app/res/values/styles.xml` - style name `QuietTV.Home` → `QuietTV.Home`
- `app/src/io.quiettv/` - all Java files, package declarations
- `build.sh` - output name, keystore names, output APK name
- `config.properties` - keep as-is (user's config)
- `config.example.properties` - keep as-is
- `web/` - all JavaScript references
- `webos/` - appinfo.json, build.py references
- `tizen/` - config.xml, build.py references
- `docs/` - all HTML, references to freemytv.io
- `README.md` - all references
- `AGENTS.md` - if references exist
- `tools/` - any references

### What to KEEP (original name only in credits/attribution):
- `LICENSE` - keep original MIT license and copyright
- `README.md` credits section
- `CLAUDE.md` references to original project
- Original copyright notice

## Phase 2: Audit UI and features (pending)
- List every screen, menu, button, and option across all platforms
- Fix every broken or dead screen/option
- Use apple-design skill for visual redesign
- Keep core behavior (shelf, drawer, switching to Original)

## Phase 3: Clean up code (pending)
- Remove unused files, dead code, commented-out code
- Replace hardcoded IP addresses, personal cities, personal keys with config or defaults
- Ensure .gitignore covers build outputs, local config, secrets

## Phase 4: README and screenshots (pending)
- Rewrite README for Quiet TV
- Add screenshot placeholders at docs/screenshots/
- Only describe features that work after Phase 2

## Phase 5: Build and test on all platforms (pending)
- Android TV/Google TV: build.sh, install via adb, verify features
- LG webOS: python3 webos/build.py, python3 webos/install.py, confirm apps in drawer
- Samsung Tizen: build with tizen/scripts, check features

## Phase 6: Publish readiness (pending)
- Bump version to 2.0.0
- Add CHANGELOG.md entry
- Ensure every platform build works from clean checkout
- Write QA.md with test results

---

## Starting Phase 1

### Immediate actions:
1. Read LICENSE - keep original copyright and license notices
2. Create PLAN.md (done)
3. Begin renaming: change package from `io.quiettv` to `io.quiettv`
4. Update all Java file package declarations
5. Update AndroidManifest.xml
6. Update build.sh
7. Update web/ JS files
8. Update webos/ files
9. Update tizen/ files
10. Update docs/ files
11. Update README.md
12. Update credits/attribution (keep original)

Let me start with the renaming work.