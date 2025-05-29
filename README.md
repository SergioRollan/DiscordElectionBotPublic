# Discord Election Bot

A powerful and flexible Discord bot for managing **anonymous elections and votes** inside your server. Ideal for roleplay, private organizations, communities, or any context where secret ballot elections are needed.

[Invite the bot to your server](https://discord.com/oauth2/authorize?client_id=1377301997417398383&permissions=277025508352&scope=bot%20applications.commands)

---

## 🗳️ Features

- ✅ Fully anonymous voting system.
- 🌐 Multi-language support (Spanish and English).
- 🏛️ Elections for any kind of position or decision.
- 📬 Private vote submission via DM.
- 📊 Transparent, real-time results for participants (when configured).
- 🔐 Optional vote verification through messages or codes.

---

## ⚙️ Configuration

The bot uses environment variables (configured in a `.env` file **not included in this repository**) to store sensitive tokens. Here's a list of required environment variables:

```env
DISCORD_TOKEN=your_bot_token
CLIENT_ID=your_client_id
GUILD_ID=optional_specific_guild_id_for_testing```

## 🌍 Language Support

The bot supports the following languages:
- 🇪🇸 Spanish (default)
- 🇺🇸 English
- FR French

Language can be changed via a configuration command or environment setting depending on your implementation.

## 💬 Commands Overview

Here are the main bot commands with usage examples:

/start-election
Starts a new election.

Options:

title – Title of the election.

candidates – List of candidates (comma separated).

voters – List of users allowed to vote.

Example:

bash
Copiar
Editar
/start-election title:"President Election" candidates:"Alice, Bob, Charlie" voters:@User1 @User2 @User3
/vote
Sends a private vote via DM.

Example:

bash
Copiar
Editar
/vote candidate:"Alice"
## 🛡️ Must be used in a private message with the bot.

/end-election
Ends the current election and publishes results.

Example:

bash
Copiar
Editar
/end-election
/status
Check election status.

## 🧪 Example Flow
An admin runs /start-election.

Eligible voters receive a DM from the bot.

They use /vote in DM to submit their vote.

Once voting ends, the admin runs /end-election to show results.

## 🚀 Hosting
You can host this bot using:

Node.js (locally)

Docker

Cloud hosting (Render, Railway, etc.)

Install dependencies:

bash
Copiar
Editar
npm install
Run the bot:

bash
Copiar
Editar
node index.js
Make sure your .env file is properly configured and placed in the root directory.

## 📂 Structure
bash
Copiar
Editar
📁 src/
├── commands/         # Slash commands definitions
├── events/           # Bot event handlers
├── logic/            # Election logic
├── lang/             # Translations (EN / ES)
├── utils/            # Utility functions
📄 index.js           # Bot entry point
🤝 Contributing
Contributions are welcome! Feel free to open issues or submit pull requests for improvements, new features, or bug fixes.

## 🛡️ Security
This repository does not include any secret tokens. All secrets should be managed via .env files and must not be committed to version control.
GitHub Push Protection will block any secrets accidentally included.

## 📄 License
MIT License

## 📬 Invite the Bot
Click the link below to invite the bot to your server:

🔗 Invite Link










