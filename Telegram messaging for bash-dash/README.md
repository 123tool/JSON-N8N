This workflow allows you to send a message in a Telegram chat via bash-dash.

Example usage: - telegram I'll be late

If you want to send a predefined message without typing it in the command line, you can replace the Text Expression in the Telegram node with a specific message. In this case, the dash command - telegram will send the predefined message to the chat.

Example bash-dash config: commands[telegram]="http://localhost:5678/webhook/telegram"
