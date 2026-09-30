# Privacy Policy – KBHelperBot

**Effective date:** September 30, 2026

KBHelperBot ("the bot") is a companion utility bot for the Discord game bot EPIC RPG. This policy explains what data the bot processes, why, and how you can have it removed.

## 1. What the bot reads

The bot uses Discord's Message Content intent to read messages and embeds, but access is limited in code:

- **Channel allowlist** – the bot only processes messages in channels explicitly added to its configuration. Messages in all other channels are ignored.
- **Author filter** – only messages sent by the EPIC RPG bot (verified by its user ID) are processed. Messages written by users or by other bots are discarded immediately.
- **User allowlist** – advanced features (hunt cooldown reminders, arena cooldown DMs, training and pet tips) work only for users who personally asked to be added.

Message content is processed only at the moment it is received, to calculate the bot's reply (for example a pet summary or time travel calculation). **Message content is never stored.**

## 2. What data is stored

The bot stores data only for users on the advanced features allowlist. For each such user, the bot's configuration file contains:

- Discord user ID
- Discord username
- Cooldown-related parameters, calculated automatically from EPIC RPG's replies to that user's game commands

These values are saved to the configuration file when the bot shuts down, so users don't have to set anything up again after a restart. No other personal data is collected or stored.

Users who are not on the allowlist have no data stored at all.

**Debug logging:** occasionally, when testing the bot, the developer enables logging of EPIC RPG messages in a single private test channel used only by the developer. These logs never include messages from other channels or servers, are used only to fix bugs, and are deleted once testing is finished.

## 3. How the data is used

Stored data is used only to provide the bot's features: calculating when a command's cooldown ends and sending reminders. The data is:

- not shared with, sold to or disclosed to any third party,
- not used for advertising, analytics or profiling,
- not used to train machine learning or AI models.

## 4. Where the data is kept and for how long

Data is kept in the bot's configuration file on the server where the bot is hosted, which only the bot's developer can access. It is kept until the user asks to be removed from the allowlist, at which point their entry is deleted.

## 5. Opting in and out

- **Advanced features** are opt-in. To join or leave, contact the developer (see below). When you leave, your entry, including your user ID, username and cooldown parameters, is deleted.
- **Basic features** (pet summary, time travel calculator) react only to EPIC RPG messages in allowed channels and store nothing. Server administrators can restrict the bot at any time through channel permissions or by removing it from the server.

## 6. Your rights

You can ask at any time what data is stored about you, request a copy of it, or request its deletion by contacting the developer.

## 7. Changes to this policy

If this policy changes, the updated version will be published at this address with a new effective date.

## 8. Contact

KB Helper is a private bot and cannot be invited publicly. All requests (joining or leaving the advanced features, adding the bot to a server, data access or deletion, questions about this policy) can be sent to the developer via Discord direct message:

- **Discord username:** Konrad
- **Discord user ID:** 317320517579177984

You can also reach the developer on any server where the bot is used.
