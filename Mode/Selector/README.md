🎮 HanZihan Project — Mode Selector

Free Fire Private Server
Custom Mode Selector by HanZihan Project

📸 Mode Selector Preview

"HanZihan Project Mode Selector" (ModeSelector.png)

✨ Features

- 10 pilihan mode permainan.
- Training Ground berada di urutan pertama.
- Konfigurasi "map_id", "game_mode", dan "match_mode".
- Pengaturan nama mode, tips, batas pemain, dan urutan tampilan.
- Dukungan konfigurasi melalui JSON override.
- Daftar game modes: Classic, Ranked, Clash Squad, Training Ground, Lone Wolf, dan Fight Club.

🗺️ Available Modes

No.| Mode| Map ID| Game Mode| Match Mode
1| Training Ground| 7| 23| 5
2| Bermuda| 1| 1| 1
3| Ranked Game| 1| 1| 2
4| Clash Squad| 1| 15| 1
5| CS-Ranked| 1| 15| 6
6| Lone Wolf| 11| 36| 1
7| Purgatory| 3| 1| 1
8| Kalahari| 4| 1| 1
9| Bermuda Remastered| 5| 1| 1
10| Clash Squad Kalahari| 4| 15| 1

📂 Configuration Files

Main Handler

src/tcp/handlers/GameOpeningInfo.js

Admin Customization Override

data/admin-customization-overrides.json

Override menggunakan struktur berikut:

{
  "gameOpeningInfo": {
    "modes": [],
    "game_modes": []
  }
}

- "modes": Mengatur daftar mode permainan dan urutannya.
- "game_modes": Mengatur ID serta nama game mode.

🛠️ Installation

1. Letakkan gambar Mode Selector dengan nama "ModeSelector.png".
2. Konfigurasikan mode di "GameOpeningInfo.js".
3. Sesuaikan "gameOpeningInfo" di file override.
4. Pastikan ID mode dan urutannya sesuai.
5. Restart TCP server setelah perubahan.
6. Uji Mode Selector melalui game client.

⚠️ Notes

- Mode yang tersedia bergantung pada kompatibilitas client dan server.
- ID mode yang benar tidak menjamin seluruh mode dapat dimainkan.
- Training Ground menggunakan "game_mode: 23" dan "match_mode: 5".
- Selalu buat backup sebelum mengubah konfigurasi.

👨‍💻 Credits

Project: HanZihan Project
Category: Free Fire Private Server
Feature: Custom Mode Selector

---

Made with ❤️ by HanZihan Project
