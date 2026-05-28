# Hi 👋, I'm Aayush Saurabh
### Real-time Communication Engineer | Flutter • SIP • WebRTC • CallKit

---

## 🧠 About Me

- 🔭 Building **production SIP + WebRTC calling systems** in Flutter
- 📡 Deep hands-on with **FreePBX, dart_sip_ua, flutter_webrtc, LiveKit**
- 🤖 Building a **local AI system** with document + web search (offline-first)
- ⚙️ Background: Mechanical → Product Design → Software Engineering
- 🌍 Contributing to the open-source tools I use in production

---

## ⚡ Currently Working On

- Production SIP + WebRTC systems in Flutter
- CallKit (iOS) + Telecom API (Android) deep integrations
- VoIP call queueing, reconnection & background handling
- Local AI developer assistant with document + web search
- Real-time communication architecture

---

## 🏆 Engineering Highlights

- Merged **4 OSS contributions** into production-used Flutter/WebRTC packages
- Built production VoIP workflows using **SIP + WebRTC**
- Integrated **iOS CallKit** and **Android Telecom APIs** from scratch
- Debugged native **Swift ↔ Flutter** plugin interop issues
- Worked on call queueing, reconnection, and background call handling

---

## 🌍 Open Source Contributions

### 📦 [flutter_callkit_incoming](https://github.com/hiennguyen92/flutter_callkit_incoming) — iOS CallKit Plugin

**[fix(iOS): actionCallAccept emits empty data on outgoing calls — #813 ✅ Merged](https://github.com/hiennguyen92/flutter_callkit_incoming/pull/813)**

- Traced a data corruption bug in `CXAnswerCallAction` triggered via `setCallConnected()`
- `self.data` singleton was overwritten with empty defaults before the event fired
- Fixed by reading from `call.data` (persisted on the `Call` object) instead — 2-line surgical fix
- Affects all outgoing calls; incoming calls were unaffected due to different code path

`Swift` `iOS CallKit` `Flutter plugin internals` `VoIP lifecycle debugging`

---

### 📦 [livekit-client-sdk-flutter](https://github.com/livekit/client.flutter) — LiveKit Flutter SDK

**[fix(android): prevent screen turning off during active video calls — #1057 ✅ Merged](https://github.com/livekit/client.flutter/pull/1057)**

- Screen timeout during active video calls caused UX interruptions on Android
- Added native `MainActivity` window flag handling to keep screen awake during calls
- Flags enabled when room is active, cleared on room disposal
- Used SDK-internal `lkPlatformIs` guard per reviewer feedback (not `Platform.isAndroid`)

`Kotlin` `Android` `Flutter` `LiveKit` `Native platform integration`

**[Fixed spelling typo in audio settings UI — #942 ✅ Merged](https://github.com/livekit/client.flutter/pull/942)**

- Corrected "Micriphone" → "Microphone" in example app audio device settings UI
- Tested on Android emulator and physical device

`Flutter` `LiveKit` `UI polish`

---

### 📦 [dart-sip-ua](https://github.com/flutter-webrtc/dart-sip-ua) — SIP UA for Flutter/WebRTC

**[fix: persist ws_uri in _saveSettings for proper SIP registration — #542 ✅ Merged](https://github.com/flutter-webrtc/dart-sip-ua/pull/542)**

- `ws_uri` was missing from `_saveSettings`, silently ignoring the user-entered WebSocket URL
- App always fell back to the hardcoded `wss://tryit.jssip.net:10443` regardless of input
- Added the missing persistence line — unblocks custom SIP server registration

`Dart` `SIP` `WebRTC` `dart_sip_ua` `WebSocket`

---

## 💼 Professional Experience

### 🏢 Rirabh Consulting Services LLP

- Working on **production-level VoIP applications**
- Implemented **SIP calling** using `dart_sip_ua`
- Integrated **CallKit (iOS)** and **Telecom APIs (Android)**
- Handling **real-time communication systems** end-to-end

---

## 🚀 Featured Projects

### 📞 VoIP Calling App
- Flutter + SIP + WebRTC calling system
- CallKit (iOS) + Android Telecom full integration
- Real-time voice/video with background call handling

### 🤖 Local AI Assistant
- Fully offline knowledge system
- PDF + web search integration
- Developer productivity tool

---

## 🔬 Technical Interests

- SIP signaling & VoIP infrastructure
- WebRTC media pipelines
- CallKit / Telecom framework internals
- Native iOS (Swift) ↔ Flutter plugin interoperability
- Local AI systems & retrieval pipelines
- Offline-first developer tools

---

## 🛠️ Tech Stack

`Flutter` `Dart` `Swift` `Kotlin` `SIP` `WebRTC` `FreePBX`  
`LiveKit` `CallKit` `Android Telecom` `Firebase` `REST APIs`  
`Python` `Blender` `Fusion 360`

---

## 📊 GitHub Stats

![Stats](https://github-readme-stats.vercel.app/api?username=mechtech-mind&show_icons=true&theme=tokyonight)
![Streak](https://streak-stats.demolab.com?user=mechtech-mind&theme=tokyonight)
![Trophies](https://github-profile-trophy.vercel.app/?username=mechtech-mind&theme=tokyonight&row=1)
![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=mechtech-mind&theme=tokyo-night)

---

## 🌐 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aayush-saurabh-b75272409/)
[![Behance](https://img.shields.io/badge/Behance-1769FF?style=for-the-badge&logo=behance&logoColor=white)](https://www.behance.net/aayushsaurabh/projects)

---

⭐ *Contributing to the real-time communication infrastructure I build on every day.*
