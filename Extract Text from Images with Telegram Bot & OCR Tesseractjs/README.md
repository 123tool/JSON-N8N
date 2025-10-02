How it Works

The workflow listens for new image messages coming in via the Telegram bot.

Once an image is received, it downloads the image file from Telegram (which initially arrives as application/octet-stream).

The image data, now properly identified, is then sent to the Tesseract OCR node to extract the text.

Finally, the recognized text is sent back as a reply to the Telegram user.

Setup Steps

Install Community Node: Ensure you have installed n8n-nodes-tesseractjs in your n8n instance.

Connect Telegram Bot: Configure the Telegram Trigger node with your Telegram bot.

Bot Token: Add your Telegram bot token to the Send Message node to send replies.

Deploy & Test: Activate (deploy) the workflow and send an image to your Telegram bot to test.

