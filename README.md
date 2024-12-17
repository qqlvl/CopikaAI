# Copika 🤖

<div align="center">
  <img src="./docs/static/img/copika.jpg" alt="Copika Banner" width="100%" />
</div>

<div align="center">

  📖 [Web  ](https://copyme.fun) &nbsp;&nbsp;| 🤖 [Twitter  ](https://x.com/CopikaAI) &nbsp;&nbsp;  | 📊 [Pump  ](https://x.com/CopikaAI)   | 👩 [Eliza](https://github.com/ai16z/eliza) &nbsp;&nbsp; | 🐐 [GOAT](https://github.com/goat-sdk/goat) &nbsp;&nbsp;

</div>

## 💠 New Features


-&nbsp;&nbsp; 💾 Parsing Solana blockchain
-&nbsp;&nbsp; 📟 On-chain analysis
-&nbsp;&nbsp; 🖇️ Copytrading 
-&nbsp;&nbsp; 🪪 Publication of transaction data and PNL




## ✨ Basic Features

-   🛠️ Full-featured Discord, Twitter and Telegram connectors
-   🔗 Support for every model (Llama, Grok, OpenAI, Anthropic, etc.)
-   👥 Multi-agent and room support
-   📚 Easily ingest and interact with your documents
-   💾 Retrievable memory and document store
-   🚀 Highly extensible - create your own actions and clients
-   ☁️ Supports many models (local Llama, OpenAI, Anthropic, Groq, etc.)
-   📦 Just works!





## 🚀 Quick Start

### Prerequisites

-   [Python 2.7+](https://www.python.org/downloads/)
-   [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
-   [pnpm](https://pnpm.io/installation)

> **Note for Windows Users:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) is required.

### Use the Starter (Recommended)

```bash
git clone https://github.com/ai16z/Copika-starter.git

cp .env.example .env

pnpm i && pnpm build && pnpm start
```

### Manually Start Copika (Only recommended if you know what you are doing)

```bash
# Clone the repository
git clone https://github.com/ai16z/Copika.git

# Checkout the latest release
# This project iterates fast, so we recommend checking out the latest release
git checkout $(git describe --tags --abbrev=0)
```

### Edit the .env file

Copy .env.example to .env and fill in the appropriate values.

```
cp .env.example .env
```

Note: .env is optional. If your planning to run multiple distinct agents, you can pass secrets through the character JSON

### Automatically Start Copika

This will run everything to setup the project and start the bot with the default character.

```bash
sh scripts/start.sh
```

### Edit the character file

1. Open `packages/core/src/defaultCharacter.ts` to modify the default character. Uncomment and edit.

2. To load custom characters:
    - Use `pnpm start --characters="path/to/your/character.json"`
    - Multiple character files can be loaded simultaneously
3. Connect with X (Twitter)
    - change `"clients": []` to `"clients": ["twitter"]` in the character file to connect with X

### Manually Start Copika

```bash
pnpm i
pnpm build
pnpm start

# The project iterates fast, sometimes you need to clean the project if you are coming back to the project
pnpm clean
```

#### Additional Requirements

You may need to install Sharp. If you see an error when starting up, try installing it with the following command:

```
pnpm install --include=optional sharp
```

### Community & contact

-   [GitHub Issues](https://github.com/ai16z/Copika/issues). Best for: bugs you encounter using Copika, and feature proposals.
