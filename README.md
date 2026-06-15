# CS2 Private Server

**Play Counter-Strike 2 Offline with Friends on LAN**

![CS2 Private Server](https://img.shields.io/badge/CS2-Private%20Server-orange?style=for-the-badge&logo=counter-strike)
![Status](https://img.shields.io/badge/Status-Active-green?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

## 🎮 Features

- ✅ **LAN Player Discovery** - Auto-detect friends on your network
- ✅ **Real-time Name Injection** - Custom player names in-game
- ✅ **Quick Connect** - Connect to players with 1-9 keys
- ✅ **Web Dashboard** - Live launcher status on website
- ✅ **Host/Join Servers** - Easy server hosting and joining
- ✅ **Anti-Bypass Protection** - Secure launcher integration
## 🌐 Websites

- **counterstrike2.com**
- **counterstrike2.net**

## 🚀 Quick Start

### 1. Download & Install

1. Download the CS2 Private Server launcher
2. Extract to your CS2 directory
3. Run as Administrator

### 2. Launch the Server

```bash
# Open CS2Launcher.exe
# Enter your player name
# Choose an option:
#   [H] Host Server
#   [P] Play (auto-connect)
#   [C] Connect to Server
#   [N] News
```

### 3. Access Web Dashboard

1. Open the launcher (console must be running)
2. Visit the website
3. See **"Logged in as [YourName]"** in the header
4. View live status: CS2 running, players on LAN

## 📡 API Integration

The launcher runs a local API server on port `27016`.

### Endpoint: `/api/status`

**Request:**
```http
GET soon
```

**Response:**
```json
{
  "status": "online",
  "playerName": "YourName",
  "cs2Running": true,
  "playersOnLAN": 2
}
```

## 🛠️ Development

### Website Setup

```bash
npm install
npm run dev
```

The website will automatically connect to the launcher API when running.

### Tech Stack

- **Launcher:** C++
- **Website:** React + TypeScript + Vite + Tailwind CSS
- **API:** ????

## 📋 Requirements

- Counter-Strike 2 installed
- Windows 10/11
- Administrator rights
- LAN connection for multiplayer

## 🎯 Coming Soon

- 🎮 Web-based Server Browser
- 👥 Player Statistics & Leaderboards
- 🗺️ Custom Map Rotation System
- 🎯 Tournament Mode
- 💬 Integrated Voice Chat
- 📊 Real-time Server Monitoring
- 🎨 Skin Generator (items.json)
- 🎯 Crosshair Generator
- ⌨️ Bind Generator

## 📝 How It Works

1. **Launcher starts** → Creates lock file for anti-bypass
2. **API server starts** → Listens on port 27016
3. **CS2 launches** → Injects custom player name
4. **Website connects** → Shows "Logged in as [Name]"
5. **LAN discovery** → Broadcasts player info on network
6. **Players connect** → Quick join with number keys

## 🔒 Security

- Administrator rights required
- Anti-bypass protection prevents CS2 from launching without launcher
- Lock file system ensures single launcher instance
- CORS enabled for local website access

## 🤝 Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

## 📄 License

MIT License - See LICENSE file for details

## 🔗 Links

- **GitHub:** https://github.com/dscdevelopers22-sketch/cs2privateserverr
- **Website:** counterstrike2server.com | counterstrike2server.net

---

**Made with ❤️ for the CS2 community**
