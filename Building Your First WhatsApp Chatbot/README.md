How it works
  - This template is in 2 parts: creating the product catalog vector store and building the WhatsApp AI chatbot.
  - A product brochure is imported via HTTP request node and its text contents extracted.
  - The text contents are then uploaded to the in-memory vector store to build a knowledgebase for the chatbot.
  - A WhatsApp trigger is used to capture messages from customers where non-text messages are filtered out.
  - The customer's message is sent to the AI Agent which queries the product catalogue using the vector store tool.
  - The Agent's response is sent back to the user via the WhatsApp node.

How to use
Once you've setup and configured your WhatsApp account and credentials
  - First, populate the vector store by clicking the "Test Workflow" button.
  - Next, activate the workflow to enable the WhatsApp chatbot.
  - Message your designated WhatsApp number and you should receive a message from the AI sales agent.
  - Tweak datasource and behaviour as required.

Requirements
  - WhatsApp Business Account
  - OpenAI for LLM

Customising this workflow
  - Upgrade the vector store to Qdrant for persistance and production use-cases.
  - Handle different WhatsApp message types for a more rich and engaging experience for customers.
