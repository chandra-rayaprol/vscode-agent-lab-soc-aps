# 🎯 Soc Ops - Social Bingo

> Break the ice, make connections, and have fun at your next social mixer!

**Soc Ops** is an interactive social bingo game designed to energize in-person events and help people connect through shared experiences. Find someone who matches each square, mark it off, and race to get 5 in a row! 🎉

[![Deploy to GitHub Pages](https://github.com/chandra-rayaprol/vscode-agent-lab-soc-aps/actions/workflows/deploy.yml/badge.svg)](https://github.com/chandra-rayaprol/vscode-agent-lab-soc-aps/actions/workflows/deploy.yml)

---

## ✨ Features

- 🎲 **5x5 Bingo Grid** - Randomly shuffled questions for a unique experience every time
- 💾 **Auto-Save Progress** - Game state persists in your browser
- 📱 **Mobile-First Design** - Optimized for phones at social events
- 🎊 **Celebration Animations** - Fun animations when you get BINGO!
- ⚡ **Lightning Fast** - Built with modern React and Vite
- 🎨 **Beautiful UI** - Styled with Tailwind CSS v4
- 🆓 **FREE SPACE** - Center square starts marked for faster gameplay

## 🎮 How to Play

1. Open the game on your mobile device
2. Mingle with other attendees at your event
3. Find people who match the descriptions in each square
4. Tap squares to mark them as you find matches
5. Get 5 in a row (horizontal, vertical, or diagonal) to win! 🏆

## 🚀 Quick Start

### Prerequisites

- [Node.js 22](https://nodejs.org/) or higher

### Installation

```bash
# Clone the repository
git clone https://github.com/chandra-rayaprol/vscode-agent-lab-soc-aps.git
cd vscode-agent-lab-soc-aps

# Install dependencies
npm install

# Start development server
npm run dev
```

Visit `http://localhost:5173` to see the game in action! 🎮

### Build for Production

```bash
npm run build
```

The built files will be in the `dist/` directory, ready to deploy.

## 🛠️ Tech Stack

- **[React 19](https://react.dev/)** - Modern UI framework
- **[TypeScript](https://www.typescriptlang.org/)** - Type-safe JavaScript
- **[Vite](https://vite.dev/)** - Next-generation frontend tooling
- **[Tailwind CSS v4](https://tailwindcss.com/)** - Utility-first CSS framework
- **[Vitest](https://vitest.dev/)** - Fast unit testing framework

## 📦 Project Structure

```
src/
├── components/       # React UI components
├── hooks/           # Custom React hooks (game logic)
├── utils/           # Pure utility functions
├── data/            # Game questions and constants
└── types/           # TypeScript type definitions
```

## 🎨 Customization

Want to customize the game for your event? Check out the **[Lab Guide](.lab/GUIDE.md)** for detailed instructions on:

- Adding or modifying questions
- Customizing colors and themes
- Adjusting game rules
- Deploying to your own domain

## 📝 Development

### Available Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm test` | Run test suite |
| `npm run lint` | Lint code with ESLint |

### Deployment

This project automatically deploys to **GitHub Pages** when you push to the `main` branch. Your game will be live at:

`https://<username>.github.io/<repo-name>/`

## 🤝 Contributing

Contributions are welcome! Please check out our [Contributing Guidelines](CONTRIBUTING.md) to get started.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 💬 Support

- 📚 [Documentation](.lab/GUIDE.md)
- 🐛 [Report Issues](https://github.com/chandra-rayaprol/vscode-agent-lab-soc-aps/issues)
- 💡 [Discussion Forum](https://github.com/chandra-rayaprol/vscode-agent-lab-soc-aps/discussions)

## 🌟 Acknowledgments

Created with ❤️ for bringing people together at social events.

---

**Ready to play?** [Launch the game now!](https://chandra-rayaprol.github.io/vscode-agent-lab-soc-aps/) 🎯
