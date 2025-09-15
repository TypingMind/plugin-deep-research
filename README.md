## Deep Research

Perform deep research on a specific topic and compile a final report with the ability to draft a research plan, search the web, and read web pages.

This plugin uses **Serp API** and **Firecrawl API**. You need to provide API keys from both services to start using it.

### Research Mode

- **Lightweight Mode**: In lightweight mode, Deep Research will attempt to extract data from online sources using the extract tool from Firecrawl, which saves tokens at a cost of reduced data accuracy. This is the default mode.
- **Comprehensive Mode**: Deep Research will read the full content of the online sources to determine the final answer. If the web pages have a lot of content, it can risk consuming a lot of tokens, which is expensive and may exceed the model's context length limit.
- **Dynamic Mode**: Deep Research will run in Lightweight Mode by default, but may opt in to read full web page content when absolutely needed to get the most accurate answer.

### Customizable
The Deep Research plugin is customizable. You can duplicate this plugin and add your own tools to enhance the quality of the final report. The system instructions and prompts are also available in the plugin source.

By default, the Deep Research plugin comes with 3 tools: Research Plan, Search Web, and Read Web Page. Depending on your specific needs, you can add more tools like reading from a tweet, searching from a private database, or controlling a browser. The TypingMind plugin system allows you to add multiple tools to the Deep Research plugin and supports various ways to implement your tools using JavaScript, HTTP requests, or MCP.

[Learn how to develop TypingMind plugins here](https://www.typingmind.com/plugins-docs).

## Token Usage
This plugin may use multiple tools in multiple turns. A deep research task can run for up to 2 minutes. Please monitor the token usage closely to avoid consuming too many tokens. You can also modify the plugin to make it more token-efficient by adding your own tools to perform web searches and read web pages.

### Example Usage

> Compare the current latest EV cars and their prices available for purchase in the EU.
