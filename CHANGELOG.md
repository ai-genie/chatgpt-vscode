# What's New?

All notable changes to the [ChatGPT](https://marketplace.visualstudio.com/items?itemName=genieai.chatgpt-vscode) extension will be documented in this file.

## 🆕 [V0.0.5] 💡 Quick fix problems - 2022-03-31

- Ask Genie to quick fix the problems that you see in your code
- Click on the lightbulb on a code piece where you see underlined error

  <img src="https://raw.githubusercontent.com/ai-genie/chatgpt-vscode/main/images/quick-fix.png" alt="Genie: Quick fix" style="max-width: 100%;max-height: 240px;">

## 🆕 [V0.0.4] 💬 Save your conversations and continue at any time - 2022-03-27

- Show conversations button is now always visible on the home page for discoverability.
- Various UX Improvements.
- You can change API Key directly from home page
- Updated documentation and added screenshots of the features available

## 🆕 [V0.0.3] - 2022-03-25

### 1. Conversation history

#### Save your conversations and continue at any time

- The goal: Collect feedback and measure the compatibility across different machine, OS setups.
- We are experimenting a new feature to help you store your conversations in your disk using VS Code global storage API.
- You need to opt-in to use this feature as this is experimental to collect feedback from the users. Setting name: `genieai.enableConversationHistory`
- With this experimental feature, keep in mind this feature has limitations at the moment and may have bugs, use it at your own risk.
- You may want to remove the stored files manually for privacy from time to time, extension doesn't have any way to modify the files other than writing new threads to files.
- All conversations start with name 'New chat' and you can change it in `genie.json` file.
- The conversations are stored only on your machine, using VS Code's provided global storage API for extensions.

### 2. Misc. bug fixes and improvements

> ### Conversation history - Demo
>
> ---
>
> <a href="https://www.loom.com/share/1a57be874e5d4ec099493cc68ed31e04">
>   <p>Genie - ChatGPT Conversation History - Watch Video</p>
>   <img style="max-width:300px;" src="https://cdn.loom.com/sessions/thumbnails/1a57be874e5d4ec099493cc68ed31e04-with-play.gif">
> </a>

---

## [0.0.1] - 2022-03-20

### New home for the most popular VS Code ChatGPT extension

- See differences between your code and AI generated code (Click `Diff` on the code block generated)
- Personalize your AI's name
- Ice breakers to get to know how capable OpenAI GPT models are.
- Editor View: Get answers in your vs-code editor instead of the chat window.
  - Set temperature for your prompt
  - Add your prompt + temperature to shortcuts to use it later

<img src="https://raw.githubusercontent.com/ai-genie/chatgpt-vscode/main/images/first-features.gif">
