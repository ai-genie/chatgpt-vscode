<h2 align="center"><img src="https://raw.githubusercontent.com/ai-genie/chatgpt-vscode/main/images/ai-logo.png" height="64"><br>A Visual Studio Code - ChatGPT Integration</h2>
<p align="center"><strong>Prompt OpenAI's GPT-4, GPT-3.5, GPT-3 and Codex models within Visual Studio Code</strong></p>
<p align="center"><strong>This repository is meant for documentation, bug reports and feature requests</strong></p>

<p align="center">
    <a href="https://marketplace.visualstudio.com/items?itemName=genieai.chatgpt-vscode" alt="Marketplace version">
        <img src="https://img.shields.io/visual-studio-marketplace/v/genieai.chatgpt-vscode?color=orange&label=VS%20Code%20Marketplace" />
    </a>
    <a href="https://marketplace.visualstudio.com/items?itemName=genieai.chatgpt-vscode" alt="Marketplace download count">
        <img src="https://img.shields.io/visual-studio-marketplace/d/genieai.chatgpt-vscode?color=blueviolet&label=Downloads" />
    </a>
    <a href="https://github.com/ai-genie/chatgpt-vscode" alt="Github star count">
        <img src="https://img.shields.io/github/stars/ai-genie/chatgpt-vscode?color=blue&label=Github%20Stars" />
    </a>
</p>

> ## Testimonials
>
> #### ❄️ Featured by [Snowflake](https://www.linkedin.com/feed/update/urn:li:share:7032091318650605568) on Medium blogpost
>
> #### 🎌 Blogpost [VSCode に ChatGPT の拡張機能を入れてコードレビューやバグを発見してもらう](https://qiita.com/tak001/items/c3000b3ce9b6e72b2ae5)
>
> #### 💙 Reviews on [Twitter](https://twitter.com/jarrodWattsDev/status/1623092184906928132)
>
> #### ❤️ ChatGPT the pair programmer - VS Code on [Youtube](https://www.youtube.com/watch?v=zWTU9xH6T70)
>
> #### 💙 Generative AI on [LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:7030732108612423681)

# Level up your developer experience with Genie

- 🆕💬 Store your conversation history on your disk and continue at any time.
- 🔁 See diff between your code and Genie's suggestion right within editor with one click.
- 👤 Rename and personalize your assistant.
- 📃 Get streaming answers to your prompt in editor or sidebar conversation.
- 🔥 Streaming conversation support and stop the response to save your tokens.
- 📝 Create files or fix your code with one click or with keyboard shortcuts.
- ➡️ Export all your conversation history at once in Markdown format.
- ➕ Use GPT-4, GPT-3.5, GPT3 or Codex models via your OpenAI API Key.

# 📣 What's new?

<details open>
  <summary><strong> Save your conversations and continue at any time</strong></summary>

1. Conversation history

- The goal: Collect feedback and measure the compatibility across different machine, OS setups.
- We are experimenting a new feature to help you store your conversations in your disk using VS Code global storage API.
- You need to opt-in to use this feature as this is experimental to collect feedback from the users. Setting name: `genieai.enableConversationHistory`
- With this experimental feature, keep in mind this feature has limitations at the moment and may have bugs, use it at your own risk.
- You may want to remove the stored files manually for privacy from time to time, extension doesn't have any way to modify the files other than writing new threads to files.
- All conversations start with name 'New chat' and you can change it in `genie.json` file.
- The conversations are stored only on your machine, using VS Code's provided global storage API for extensions.

2. Misc. bug fixes and improvements

> ### Conversation history - Demo
>
> ---
>
> <a href="https://www.loom.com/share/1a57be874e5d4ec099493cc68ed31e04">
> <p>Genie - ChatGPT Conversation History - Watch Video</p>
>  <img style="max-width:300px;" src="https://cdn.loom.com/sessions/thumbnails/1a57be874e5d4ec099493cc68ed31e04-with-play.gif">
> </a>

</details>

---

# Get Started

Get your API Key from here: [OpenAI](https://beta.openai.com/account/api-keys)

1. Simply ask any coding question by selecting a code fragment.
2. Once asked, provide your API Key.

See below for the models that are available via API:

| Available model    | Description                                                                                                                               | Max token | Knowledge |
| :----------------- | :---------------------------------------------------------------------------------------------------------------------------------------- | :-------- | :-------- |
| gpt-4              | More capable than any GPT-3.5 model, able to do more complex tasks, and optimized for chat.                                               | 8,192     | Sep 2021  |
| gpt-4-32k          | Same capabilities as the base gpt-4 mode but with 4x the context length.                                                                  | 32,768     | Sep 2021  |
| gpt-3.5-turbo      | Most capable GPT-3.5 model and optimized for chat at 1/10th the cost of `text-davinci-003`.                                               | 4,096     | Sep 2021  |
| gpt-3.5-turbo-0301 | Snapshot of `gpt-3.5-turbo` from March 1st 2023.                                                                                          | 4,096     | Sep 2021  |
| text-davinci-003   | Can do any language task with better quality, longer output, and consistent instruction-following than the curie, babbage, or ada models. | 4,000     | Jun 2021  |
| text-davinci-002   | Similar capabilities to `text-davinci-003` but trained with supervised fine-tuning instead of reinforcement learning                      | 4,000     | Jun 2021  |
| code-davinci-002   | Optimized for code-completion tasks                                                                                                       | 4,000     | Jun 2021  |
| code-cushman-001   | Almost as capable as Davinci Codex, but slightly faster. This speed advantage may make it preferable for real-time applications.          | 2,048     |           |

## Features

The extension comes with context menu commands, copy/move suggested code into editor with one-click, conversation window and customization options for OpenAI's ChatGPT prompts.

- 📤 Export all your conversation history with one click
- Ad-hoc prompt prefixes for you to customize what you are asking ChatGPT
- Customize what you are asking with the selected code. The extension will remember your prompt for subsequent questions.
- Automatic partial code response detection. If AI doesn't finish responding, you will have the option to continue and combine answers
- 🍻 Optimized for dialogue
- Edit and resend a previous prompt
- Copy or insert the code ChatGPT is suggesting right into your editor.

## Customization

- You can enable/disable all of your context menu items. Simply go to settings and find the prompt that you would like to disable. Custom prompts are hidden by default.
- `Genie: Ad-hoc prompt`: Ad-hoc custom prompt prefix for the selected code. Right click on a selected block of code, run command.
  - You will be asked to fill in your preferred custom prefix and the extension will remember that string for your subsequent ad-hoc queries.
- `Genie: Add tests`: Write tests for you. Right click on a selected block of code, run command.
  - "default": "Implement tests for the following code",
  - "description": "The prompt prefix used for adding tests for the selected code"
- `Genie: Find bugs`: Analyze and find bugs in your code. Right click on a selected block of code, run command.
  - "default": "Find problems with the following code",
  - "description": "The prompt prefix used for finding problems for the selected code"
- `Genie: Optimize`: Add suggestions to your code to improve. Right click on a selected block of code, run command.
  - "default": "Optimize the following code",
  - "description": "The prompt prefix used for optimizing the selected code"
- `Genie: Explain`: Explain the selected code. Right click on a selected block of code, run command.
  - "default": "Explain the following code",
  - "description": "The prompt prefix used for explaining the selected code"
- `Genie: Add comments`: Add comments for the selected code. Right click on a selected block of code, run command.
  - "default": "Add comments for the following code",
  - "description": "The prompt prefix used for adding comments for the selected code"
- `Genie: Custom prompt 1`: Your custom prompt 1. It's disabled by default, please set to a custom prompt and enable it if you prefer using customized prompt
  - "default": "",
- `Genie: Custom prompt 2`: Your custom prompt 2. It's disabled by default, please set to a custom prompt and enable it if you prefer using customized prompt
  - "default": "",
- `Genie: Generate code`: If you select a Codex model (`code-*`) you will see this option in your context menu. This option will not feed the ChatGPT with any context like the other text completion prompts.

## Other available commands

- `Genie: Clear API Key`: Clears the API Key from VS Code [Secrets Storage](https://code.visualstudio.com/api/references/vscode-api#SecretStorage)
- `Genie: Ask anything`: Free-form text questions within conversation window.
- `Genie: Reset session`: Clears the current session and resets your connection with ChatGPT
- `Genie: Clear conversation`: Clears the conversation window and resets the thread to start a new conversation with ChatGPT.
- `Genie: Export conversation`: Exports the whole conversation in Markdown for you to easily store and find the Q&A list.

# Troubleshooting

## FAQ

- Re-enter API key: use `Genie: Clear API Key` command. Click `Commands` on the home page to see all commands available
- Proxy support: See this issue to enable local proxy: #7
- Usage in Remote environments: See this issue about remote/SSH: #3
- Unable To Use GPT-4 Models: You need GPT-4 API Access (Different than GPT-4 on ChatGPT Plus subscription) #6

## Common Issues

- It's possible that OpenAI systems may experience issues responding to your queries due to high-traffic from time to time.
- If you get `HTTP 429 Too Many Requests`, it means that you are making Too Many Requests. Please wait and try again in a few moments. If it persists, restart your vs-code.

  - This could be due to `insufficient_quota` on your OpenAI account. You could run the following cURL command to check if your account has enough quota. (Make sure to replace `$OPENAI_API_KEY` with your key that you use in this extension)

  ```bash
    curl https://api.openai.com/v1/completions \
      -H "Content-Type: application/json" \
      -H "Authorization: Bearer $OPENAI_API_KEY" \
      -d '{
      "model": "text-davinci-003",
      "prompt": "Can I make a request?\n\n",
      "temperature": 0.7,
      "max_tokens": 256,
      "top_p": 1,
      "frequency_penalty": 0,
      "presence_penalty": 0
    }'
  ```

- If you get `HTTP 404 Not Found` error, it means one of the parameters you provided is unknown (i.e. `genieai.openai.model`). Most likely switching to default `model` in your settings would fix this issue.
- If you get `HTTP 400 Bad Request` error, it means that your conversation's length is more than GPT/Codex models can handle. Or you supplied an invalid argument via customized settings.
- If you encounter persistent issues with your queries
  - Try `Genie: Reset session` to clear your session/conversation or `Genie: Clear API Key` to clear your API Key and re-enter
  - As a last resort try restarting your VS-Code and retry logging in.
- If you are using Remote Development and cannot use ChatGPT
  - In `settings.json` add `"remote.extensionKind": {"genieai.chatgpt-vscode": ["ui"]}`

# Disclaimer and Credits

- There is no guarantee that the extension will continue to work as-is without any issues or side-effects. Please use it at your own risk.
- This extension never uses/stores your personally identifiable information.
- This extension collects metadata to improve its features. No personally identifiable information is collected. You can opt-out from telemetry either by setting the global 'telemetry.telemetryLevel' or 'genieai.telemetry.disable'. The extension will respect both of these settings and will collect metadata only if both allow telemetry. We use the official telemetry package provided by the vscode team [here](https://github.com/Microsoft/vscode-extension-telemetry) to understand this extension's usage patterns to better plan new feature releases.
- We assume no responsibility of any issues that you may face using this extension. Your use of OpenAI services is subject to OpenAI's [Privacy Policy](https://openai.com/privacy/) and [Terms of Use](https://openai.com/terms/).
- 💻 OpenAI: https://openai.com/
- 🧪 Uses [NodeJS OpenAI API wrapper](https://github.com/transitive-bullshit/chatgpt-api)
