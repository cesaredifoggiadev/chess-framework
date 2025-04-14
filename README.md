
# ♟️ ChessChain Frontend

**ChessChain Frontend** is the modular frontend of the ChessChain ecosystem — a blockchain-powered chess platform. This project includes web components to display and manage chess games, integrate with smart contracts, and optionally play against an AI.

---

## 🚀 Features

- ✅ Fully interactive `<chess-board>` web component  
- 🧠 AI opponent (via backend API integration)  
- 🔗 Blockchain integration with MetaMask (via ethers.js)  
- 🏆 On-chain ranking visualization  
- 📜 Game history and move list  
- 🌐 Easily embeddable components in any web app  

---

## 🧱 Tech Stack

- **Vue.js 3** + Composition API  
- **TypeScript**  
- **Lit** or native **Web Components**  
- **Vite** for development & build  
- **Ethers.js** for blockchain interactions  
- **Pinia** for state management (optional)  
- **Tailwind CSS** for UI (optional)

---

## 📦 Project Structure

```
chesschain-frontend/
├── src/
│   ├── components/           # Vue components (wrappers, layout)
│   ├── web-components/       # Pure Web Components (e.g. <chess-board>)
│   ├── views/                # Pages (Game, Home, Profile)
│   ├── services/             # API + Blockchain services
│   ├── stores/               # Global state (Pinia)
│   └── utils/                # Chess logic helpers, validation, etc.
├── public/                   # Static assets
├── vite.config.ts
└── README.md
```

---

## 🧪 Getting Started

### 📥 Install dependencies

```bash
pnpm install
# or
npm install
```

### 🛠 Start development server

```bash
pnpm dev
# or
npm run dev
```

---

## 🧠 Web Components

| Component        | Description                           |
|------------------|---------------------------------------|
| `<chess-board>`  | Interactive board (move pieces, show turns) |
| `<chess-match>`  | Manages an entire match               |
| `<chess-controls>` | Buttons for reset, undo, etc.      |

These components are built to be **framework-agnostic** and can be embedded in any web page.

---

## 🔗 Blockchain Integration

- Uses `ethers.js` to:
  - Connect with wallet (MetaMask)
  - Interact with smart contracts (`ChessGame.sol`, `MatchFactory.sol`)
- Auto-detects chain and network
- Emits events to the UI (e.g., move confirmed, match ended)

---

## 🌍 Environment Variables

Create a `.env` file with the following:

```env
VITE_BACKEND_API_URL=https://api.chesschain.xyz
VITE_CONTRACT_ADDRESS=0xYourContractAddress
VITE_CHAIN_ID=137
```

---

## 🧱 TODO / Next Steps

- [ ] Add PWA support  
- [ ] Optimize mobile UX  
- [ ] Add multi-language support  
- [ ] Integrate tournament mode  

---

## 📄 License

MIT — © ChessChain Team

---

## 🤝 Contributing

Pull requests are welcome! If you want to contribute, fork the repo and submit a PR with a clear description of your changes.

---

## 📬 Contact

For questions or suggestions, open an issue or contact us at **info@deepindev.com**
