**PanterAI Telegram Bot**

This is a Telegram bot for **PanterAI**, designed to assess if **PanterAI** is a fit as an investor for your idea. The bot guides users through a series of questions and collects their responses, including uploading PDF files to Google Drive.

### Features
- Collects user information through a series of questions
- Allows users to upload PDF files
- Stores user responses and uploads files to Google Drive
- Supports skipping questions and going back to previous questions
- Sends a summary of the user's responses to a specified Telegram chat group

### Prerequisites
- Node.js (v14 or later)
- npm (v6 or later)
- A Telegram bot token
- Google Drive API credentials

### Installation
Clone the repository:

```bash
git clone https://github.com/yourusername/panterai-tg-bot.git
cd panterai-tg-bot
```

Install the dependencies:

```bash
npm install
```

Create a .env file in the root directory and add your environment variables:

```
BOT_TOKEN=your_telegram_bot_token
GOOGLE_DRIVE_FOLDER_ID=your_google_drive_folder_id
TARGET_CHAT_ID=your_target_chat_id
```

Add your Google Drive API credentials in a file named googleApiKeyFile.json in the root directory.

### Usage
To start the bot, run the following command:

```bash
node index.js
```

### Bot Commands
- `/start`: Start the bot and begin the questionnaire.
- `Abort`: Abort the current operation.
- `Back`: Go back to the previous question.
- `Skip`: Skip the current question (if applicable).

### File Structure
- `index.js`: Main bot logic and flow.
- `data/userAnswers.json`: Stores user responses.
- `download/`: Directory to store downloaded PDF files.

### Contributing
Contributions are welcome! Please open an issue or submit a pull request.

### License
This project is licensed under the MIT License. 
