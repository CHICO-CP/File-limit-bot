# Telegram File Limit Bot

This Telegram bot limits the number of files a user can send in a group to 3. If a user exceeds this limit, they will be temporarily blocked from sending files for 12 hours.

## Features

- Limits users to sending a maximum of 3 files.
- Blocks users for 12 hours if they exceed the file limit.
- Allows exceptions for specified users or groups.
- Simple commands for user interaction:
  - `/start`: Welcomes the user and explains the bot's functionality.
  - `/help`: Provides information about the file limit and blocking policy.

## Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/CHICO-CP/File-limit-bot.git
   ```
   **You enter the Bot's folder**
   ```bash
   cd File-limit-bot
   ```

2. Install the required packages: Make sure you have Python installed. You can install the required libraries using pip:
```bash
pip install pyTelegramBotAPI
```

3. Configuration:

Run the script. If API.json does not exist, you will be prompted to enter the bot token, allowed group ID, and allowed private chat ID.

Ensure that users.json is present to store user data and file limits.

***Usage***

Start the bot by running:
```bash
python bot.py
```
The bot will respond to file uploads and enforce the file limits accordingly.

# Example JSON Files

**API.json:**
```bash
{
    "token": "YOUR_BOT_TOKEN",
    "group_id": "GROUP_ID",
    "exempt_user_id": "USER_ID"
}
```

**users.json:**
```bash
{
    "user_id_1": {
        "sent_files": 2,
        "remaining_files": 1
    },
    "user_id_2": {
        "sent_files": 1,
        "remaining_files": 2
    }
}
```

#Developer

**Developer by: @DevPhant0m**

**Channel: @TEAM_CHICO_CP**
