rn-ass-player/
├── app/ # Expo Router pages
│ ├── _layout.tsx
│ ├── index.tsx
│ └── player.tsx
├── components/
│ └── VideoPlayer/
│ ├── VideoPlayer.native.tsx # Mobile player
│ ├── VideoPlayer.web.tsx # Web player
│ └── types.ts
├── public/
│ └── media/
│ ├── sample.mp4 # Demo video
│ └── subtitles.ass # Subtitles
├── scripts/ # Subtitle helpers
│ └── copy-octopus.js
├── package.json
├── tsconfig.json
└── App.tsx


---

## 🚀 Getting Started

### 1️⃣ Clone repo
```bash
git clone https://github.com/YOUR_USERNAME/rn-ass-player.git
cd rn-ass-player

2️⃣ Install dependencies
npm install
# or
yarn install

3️⃣ Run on Mobile (iOS/Android)
npx expo start


Then press:

i → open iOS simulator

a → open Android emulator

or scan QR → run on Expo Go

4️⃣ Run on Web
npx expo start --web


Expo will open your browser at http://localhost:19006.
👉 Don’t use http://localhost:8081 (that’s Metro Bundler, not a web server).

🎬 Usage Example
import VideoPlayer from "@/components/VideoPlayer";
import type { PlayerSource } from "@/components/VideoPlayer/types";

const source: PlayerSource = {
  uri: "/media/sample.mp4",
  subtitles: "/media/subtitles.ass",
};

export default function PlayerScreen() {
  return <VideoPlayer source={source} />;
}

🛠 Tech Stack

Expo (React Native + Web)

TypeScript

react-native-video

subtitle-octopus

✅ Notes

Static files (videos, subtitles) should be inside public/media for web.

On mobile, use require() or remote URLs.

Subtitles require subtitle-octopus.

📜 License

MIT License © 2025 [Your Name]


---

⚡ Tip: After you create this `README.md`, push it to GitHub and it’ll be shown on your repo page.  

👉 Do you want me to also add **badges** (like Expo, TypeScript, MIT License) at the top of the README for GitHub flair?
