# AINative Studio

<div align="center">
  <img
    src="./ainative-studio/ai_native_studio_icons/ai_native_studio_512x512.png"
    alt="AINative Studio Logo"
    width="200"
    height="200"
  />
  <p>AI-Native Development Environment</p>
</div>

AINative Studio is a powerful, open-source AI-Native development environment with built-in AI capabilities, forked from Void Editor and VS Code.

## 🛠️ Development Scripts

For developers working on AINative Studio, use these convenient scripts in the `ainative-studio/` directory:

```bash
cd ainative-studio

# Full development setup (first time or when dependencies change)
./dev-start.sh      # Installs dependencies, builds, and runs with watch mode

# Quick start (when already built)
./dev-quick.sh      # Just starts the application (faster)

# Stop all development processes
./dev-stop.sh       # Stops watch processes and application
```

## ✨ Features

- AI-powered code completion and generation
- Built-in AI chat assistant
- Advanced code navigation and refactoring
- Cross-platform support (Windows, macOS, Linux)
- Extensible architecture with a rich extension ecosystem

## Project Structure

- `ainative-studio/` - The main IDE application (forked from Void Editor)
  - See [ainative-studio/README.md](ainative-studio/README.md) for detailed development setup
- `prd.md` - Product Requirements Document
- `dev_checklist.md` - Development checklist for the rebranding process

## 🚀 Quick Start

### Prerequisites

- Node.js 18.x or later (20.x recommended)
- npm 9.x or later
- Git
- Python 3.x (for native dependencies)
- Build tools for your platform

### Installation

**Linux:**
```bash
# 1. Install correct Node.js version
nvm install
nvm use

# 2. Install Node.js global tools
npm install -g node-gyp

# 3. Install build dependencies
sudo apt-get install build-essential g++ libx11-dev libxkbfile-dev libsecret-1-dev libkrb5-dev python-is-python3

# 4. Clone repository
git clone https://github.com/AINative-Studio/AINativeStudio-IDE.git
cd AINativeStudio-IDE/ainative-studio

# 5. Install dependencies
npm install

# 6. Build React components
NODE_OPTIONS="--max-old-space-size=8192" npm run buildreact

# 7. Start build process and run application
npm run watch
# Wait until compilation completes with 0 errors, then run:
./scripts/code.sh
```

**macOS:**
```bash
# Prerequisites: Python and Xcode Command Line Tools
# If you don't have Xcode tools: xcode-select --install

nvm install
nvm use
git clone https://github.com/AINative-Studio/AINativeStudio-IDE.git
cd AINativeStudio-IDE/ainative-studio
npm install
NODE_OPTIONS="--max-old-space-size=8192" npm run buildreact
npm run watch
# Wait until compilation completes, then run:
./scripts/code.sh
```

**Windows:**
```bash
# Prerequisites: Install Visual Studio 2022 with C++ development tools
# See ainative-studio/README.md for detailed Windows setup

nvm install
nvm use
git clone https://github.com/AINative-Studio/AINativeStudio-IDE.git
cd AINativeStudio-IDE/ainative-studio
npm install
NODE_OPTIONS="--max-old-space-size=8192" npm run buildreact
npm run watch
# Wait until compilation completes, then run:
./scripts/code.bat
```

For detailed platform-specific setup and troubleshooting, see the [ainative-studio README](ainative-studio/README.md).

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please read our [Contributing Guide](https://github.com/AINative-Studio/AINativeStudio-IDE/blob/main/ainative-studio/HOW_TO_CONTRIBUTE.md) for details on our code of conduct and the process for submitting pull requests.

## 📬 Contact

For support or questions, please open an issue in our [issue tracker](https://github.com/AINative-Studio/AINativeStudio-IDE/issues).

---

<p align="center">
  Made with ❤️ by AINative Studio
</p>
