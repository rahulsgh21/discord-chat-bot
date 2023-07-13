# Discord Ping Bot

## Description
This project implements a simple Discord bot called "Discord Ping Bot" using the Go programming language. The bot responds to specific messages in a Discord server and performs actions accordingly. It uses the DiscordGo library to interact with the Discord API.

## File Structure
- **main.go**: The entry point of the application. It initializes the bot and starts its execution.
- **config.go**: Handles reading and parsing the configuration file (`config.json`) that contains the bot's settings such as token and prefix.
- **bot.go**: Contains the main logic of the Discord bot. It connects to the Discord API, listens for incoming messages, and responds to specific commands.

## Dependencies
- **github.com/akhil/discord-ping/bot**: External package for the Discord bot functionality.
- **github.com/akhil/discord-ping/config**: External package for reading and parsing the configuration file.

## Usage
1. The `ReadConfig` function in `config.go` reads the `config.json` file and extracts the bot's token and prefix. Make sure to provide a valid token for the bot to connect to Discord.
2. The `Start` function in `bot.go` initializes the Discord bot, sets up event handlers, and opens a connection to the Discord API.
3. The `messageHandler` function in `bot.go` defines the bot's behavior when receiving messages. It responds with predefined messages based on specific commands.

## Setup and Execution
1. Ensure you have Go installed on your machine.
2. Clone the project repository.
3. Update the `config.json` file with your Discord bot token and desired prefix.
4. Run the following command in the terminal to start the bot:

## Note
Make sure to import the required external libraries (`github.com/akhil/discord-ping/bot` and `github.com/akhil/discord-ping/config`) before building or running the project.

Feel free to customize and enhance the bot's functionality to suit your needs.