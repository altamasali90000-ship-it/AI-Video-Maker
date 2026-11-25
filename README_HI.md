# AI Video Maker — Android Starter Project

## इसमें क्या है
- Android WebView app shell
- Hindi script input
- 3D Cartoon / 2D Cartoon / Realistic Human / Auto style selector
- 100 voice selection slots
- 1 या 2 मिनट duration
- 720p / 1080p / 1440p / 2160p quality selector
- 9:16 / 16:9 / 1:1 format
- Optional photo upload preview
- Local demo counter (20/day)

## जरूरी सीमा
यह starter UI prototype है, पूरा AI video generation backend नहीं। Generate बटन अभी डेमो संदेश देता है। असली generation के लिए server/API integration चाहिए:
1. Script-to-scene planner (script को scenes, characters, locations और prompts में बदले)
2. Image generation service
3. Image-to-video / text-to-video service
4. Text-to-speech service with licensed voices
5. Video stitching, subtitles, music और MP4 rendering
6. Server-side daily quota (20 successful jobs/day/user)

1440p और 2160p तभी उपलब्ध होंगे जब चुना गया generation/rendering provider इन resolutions को सपोर्ट करे। 20 free videos/day की गारंटी केवल UI से संभव नहीं; provider quota और compute cost पर निर्भर है।

## Android Studio में खोलना
1. ZIP extract करें।
2. Android Studio में `AI_Video_Maker_Android` folder खोलें।
3. Gradle sync करें (Android Gradle Plugin 8.7.3; SDK 35).
4. USB debugging enabled Android phone जोड़ें और Run दबाएँ।
5. APK बनाने के लिए Build > Build Bundle(s) / APK(s) > Build APK(s).

## अगला development चरण
Backend endpoint और provider credentials server पर configure करने के बाद WebView UI से secure HTTPS API call जोड़ें। API keys कभी APK/HTML में hardcode न करें।
