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

### `/create`
Create a new election. Users can apply as candidates by reacting to the message.

**Example:**
```bash
/create name: Lineup for tomorrow NBA finals
```
- The election name must be unique.
- The bot will post a message where users can react to apply.
- The message updates dynamically as users apply.

---

### `/open`
Open an election for voting, specifying the maximum votes per user.

**Example:**
```bash
/open name: Lineup for tomorrow NBA finals max_votes: 5
```
- Only admins or users with the configured role can open elections.
- The bot will post the list of candidates and instructions for voting. Each candidate will have a number next to their name.
- In this case, since basketball lineups are made of 5 players, we will want each person to vote for 5 people

---

## `/vote`
Vote for your preferred candidates. Use numbers separated by commas or spaces.

**Example:**
```bash
/vote name: Lineup for tomorrow NBA finals votes: 1,3
```
- You can only vote for open elections.
- The number of votes must not exceed the maximum allowed.
- Votes are anonymous (except for admins, explained later).
- In the example, the user casts their vote to the first and third applicants.

---

## `/close`
Close an election and display the winners (including ties) and results.

**Example:**
```bash
/close name: Lineup for tomorrow NBA finals winners: 5
```
- Only admins or users with the configured role can close elections.
- The bot will announce the winners and show the results.
- In this example, we will want the 5 players with the most votes, so that they make the match lineup.

---

## `/view`
Privately view the votes of each user (admin only).

**Example:**
```bash
/view name: Lineup for tomorrow NBA finals
```
- Results are sent as a private message to the admin, no one else will be able to read it even if in the same channel.
- Can only be used after opening and before closing the election

---

## `/delete`
Delete an election (admin or authorized role only).

**Example:**
```bash
/delete name: Lineup for tomorrow NBA finals
```

---

## `/config`
Configure the admin role for managing elections (admin only).

**Example:**
```bash
/config role: "Election Manager"
```
- Role name is case-insensitive and ignores spaces.

---

## `/language`
Change the bot language (admin only).

**Example:**
```bash
/language lang: "en"
```
- Options are: "Español" for Spanish, "English" for English, "Français" for French

---

## `/state`
Show the current bot state, including: language, admin role, created/open elections (admin only).

**Example:**
```bash
/state
```

---

## `/help`
Show help adapted to the user's permissions.

- Admins see all commands.
- Authorized role sees all except admin-only commands.
- Regular users see only `/help`, `/contact`, and `/vote` (with example).

---

## `/contact`
Show a private message with the bot creator's contact.

**Example:**
```bash
/contact
```

---

# Autocomplete

- All commands with an election name parameter support dynamic autocompletion.
- Only relevant elections are shown (e.g., only open elections for `/vote`).

---

# Configuration

- **Admin Role:** Set with `/config`. Only admins can change it.
- **Language:** Set with `/language`. Only admins can change it.
- **Permissions:** Only users with the configured role or admin can manage elections.

---


# Example Workflow

1. **Create an election:**
   ```bash
   /create name: "Best Moderator"
   ```
2. **Users apply as candidates by reacting.**
3. **Open the election for voting:**
   ```bash
   /open name: "Best Moderator" max_votes: 2
   ```
4. **Users vote:**
   ```bash
   /vote name: "Best Moderator" votes: 1,2
   ```
5. **Close the election:**
   ```bash
   /close name: "Best Moderator"
   ```

---

# Support

For questions or issues, use `/contact` in your server to get in touch with the creator.


---

## 📬 Invite the Bot
Click the link below to invite the bot to your server:

🔗 [Invite Link](https://discord.com/oauth2/authorize?client_id=1377301997417398383&permissions=277025508352&scope=bot%20applications.commands)










