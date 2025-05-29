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

## 🌍 Language Support

The bot supports the following languages:
- 🇪🇸 Spanish (default)
- 🇺🇸 English
- FR French

Language can be changed via a configuration command or environment setting depending on your implementation.

---

## 💬 Commands Overview

Commands & Usage
/create
Create a new election. Users can apply as candidates by reacting to the message.
Example:
Apply to deploy-comma...
The election name must be unique.
The bot will post a message where users can react to apply.
The message updates dynamically as users apply.
/open
Open an election for voting, specifying the maximum votes per user.
Example:
Apply to deploy-comma...
Only admins or users with the configured role can open elections.
The bot will post the list of candidates and instructions for voting.
/vote
Vote for your preferred candidates. Use numbers separated by commas or spaces.
Example:
Apply to deploy-comma...
You can only vote for open elections.
The number of votes must not exceed the maximum allowed.
Votes are anonymous.
/close
Close an election and display the winners (including ties) and results.
Example:
Apply to deploy-comma...
Only admins or users with the configured role can close elections.
The bot will announce the winners and show the results.
/view
Privately view the votes of each user (admin only).
Example:
Apply to deploy-comma...
Results are sent as a private message to the admin.
/delete
Delete an election (admin or authorized role only).
Example:
Apply to deploy-comma...
/state
Show the current bot state: language, admin role, created/open elections (admin only).
Example:
Apply to deploy-comma...
/config
Configure the admin role for managing elections (admin only).
Example:
Apply to deploy-comma...
Role name is case-insensitive and ignores spaces.
/language
Change the bot language (admin only).
Example:
Apply to deploy-comma...
/help
Show help adapted to the user's permissions.
Admins see all commands.
Authorized role sees all except admin-only commands.
Regular users see only /help, /contact, and /vote (with example).
/contact
Show a private message with the bot creator's contact.
Example:
Apply to deploy-comma...
Autocomplete
All commands with an election name parameter support dynamic autocompletion.
Only relevant elections are shown (e.g., only open elections for /vote).
Configuration
Admin Role: Set with /config. Only admins can change it.
Language: Set with /language. Only admins can change it.
Permissions: Only users with the configured role or admin can manage elections.
Deployment
Clone the repository.
Install dependencies:
Apply to deploy-comma...
Deploy commands to your server:
Apply to deploy-comma...
Start the bot:
Apply to deploy-comma...
Example Workflow
Create an election:
/create name: "Best Moderator"
Users apply as candidates by reacting.
Open the election for voting:
/open name: "Best Moderator" max_votes: 2
Users vote:
/vote name: "Best Moderator" votes: 1,2
Close the election:
/close name: "Best Moderator"
View results or delete as needed.
Support
For questions or issues, use /contact in your server to get in touch with the creator.
License
MIT
If you have any questions or suggestions, feel free to open an issue or contact the maintainer!


---

## 📬 Invite the Bot
Click the link below to invite the bot to your server:

🔗 Invite Link










