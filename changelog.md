# Changelog

## v1.0.1 — Stability Fix ⚡
**Release Date:** October 09, 2026

### 🔧 Fixed
- **Facebook / Messenger crash** after install — app-specific bind mount removed
- **Instagram crash** on story reply picker — Instagram lock removed  
- **TikTok crash** — TikTok lock removed
- **Boot hang / screen freeze** on some devices — nested find operations removed
- **Extra GMS services disable** reverted to only essential services
- **Boot time** improved by ~20 seconds on heavy devices

### ✨ Improved
- Auto cleanup before reinstall — prevents old corrupt font files
- Dynamic `module.prop` reading — name / version / author auto-updates
- Logging system added (`/data/adb/modules/iOSx69/iOSxAnd.log`)
- Safer `bind_font()` — no empty file creation, no data loss
- Timeout protection in `wait_for_boot()` — prevents infinite loop

### 🗑️ Removed
- Instagram explicit lock (caused crash)
- TikTok explicit lock (caused crash)
- Facebook / Messenger font download block (caused hang)
- Extra GMS services (FontsUpdateService, FontsService)
- Nested find operations (CPU overload)

### 🎯 Result
- ✅ All apps open normally (FB, Insta, TikTok, Messenger)
- ✅ System-wide iOS emoji still works
- ✅ No crash, no hang, no boot loop
- ✅ Stable on all Android versions 10–16
- ✅ Works on Magisk / KernelSU / KernelSU Next / SukiSU / APatch

---

## v1.0.0 — Initial Release 🌱
**Release Date:** October 08, 2026

### ✨ Features
- iOS emoji system-wide replace
- Kohinoor Bangla font
- Facebook / Messenger / Instagram / TikTok support
- Gecko (Firefox) support
- GMS font override blocked
- Mainstream BD brands supported
- No daemon, no battery drain
- Magisk / KernelSU / KernelSU Next / SukiSU / APatch support