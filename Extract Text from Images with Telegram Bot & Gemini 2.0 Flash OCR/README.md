Description
Turn your Telegram bot into a powerful OCR (Optical Character Recognition) tool. This workflow allows you to send any image (like a screenshot, a photo of a document, or a picture of a sign) to your bot, and it will instantly extract and send back the text from that image.

Powered by Google's advanced Gemini AI, this automation is perfect for quickly digitizing notes, saving important snippets, or avoiding manual typing.

How it works

This workflow performs a few high-level steps:

It triggers when a new image is sent to your Telegram bot.
It sends the image to the Google Gemini Vision API to be analyzed.
It extracts the text found in the image.
It sends the extracted text back to you as a message in Telegram.
Set up steps

Estimated set up time: Less than 5 minutes.

The setup is straightforward. You only need to configure two credentials:

Telegram Bot Credentials: To connect your bot.

Google Gemini API Credentials: To use the OCR feature. You can get a free API key from Google AI Studio.
