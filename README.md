🎨 Marker: AI Chat
Marker is a sleek, lightweight, fully-featured, and responsive AI chat client that runs entirely in the browser. It features a neo-brutalist design aesthetic, supports multiple AI providers, and keeps all of your API keys and chat histories securely stored in your browser's local storage.

✨ Features
Multi-Provider Support: Seamlessly switch between popular AI backends:

Google Gemini (gemini-2.5-flash, pro, etc.)

OpenAI (gpt-4o, gpt-4o-mini, etc.)

Anthropic Claude (claude-sonnet, haiku)

OpenRouter

Groq

Custom OpenAI-compatible local servers (Ollama, LM Studio, vLLM)

Bring Your Own Key (BYOK): Your API keys never touch a backend server; they are stored locally on your machine (localStorage).

Rich Markdown & Syntax Highlighting: Renders headers, lists, blockquotes, tables, and formatted code blocks with a built-in lightweight tokenizer and a copy-to-clipboard utility.
Token Tracking: Real-time monitoring of input and output token usage per message and per chat session.

Customizable Parameters: Adjust creativity/temperature slider and set custom system instructions.

Chat History: Automatically saves, renames, and manages multiple conversation threads locally with delete confirmations.

Responsive & Accessible: Fully optimized for both desktop and mobile devices, including safe-area inset support for modern mobile browsers.


🚀 Getting Started

Because Marker is built as a single-file web application, you do not need to install Node.js, run a build step, or configure a backend server.

Option 1: Run Locally

Copy the HTML code and save it as index.html.

Double-click the file to open it in any modern web browser (Chrome, Safari, Firefox, Edge).


Option 2: Host Static
You can deploy this single index.html file instantly to static hosting providers like:

GitHub Pages

Vercel

Netlify

Cloudflare Pages

🔑 How to Use

Add an API Key:

Click on the Settings button in the bottom-left sidebar (or click the model badge in the header).

Select your preferred AI Provider.

Paste your API key (optional for local servers like Ollama).

Click Test key to verify connection and fetch available models, then click Save.

Start Chatting:

Type your prompt in the text area at the bottom.

Press Enter to send, or Shift + Enter to add a new line.


Manage Chats:

Click New chat to start a fresh conversation (or use shortcut Ctrl/Cmd + K).

Access previous chats from the sidebar history. Hover over a chat to reveal the delete button.


🛠️ Built With

HTML5 / CSS3 (Vanilla implementation)

Tailwind CSS (via CDN for utility classes)

Google Fonts: Bricolage Grotesque & JetBrains Mono

Vanilla JavaScript (ES6+) utilizing Async Generators for handling Server-Sent Events (SSE) streaming responses.


🔒 Privacy & Security

Client-Side Only: Marker does not use an intermediate proxy server. All API requests are made directly from your browser to the respective AI provider's API.
Local Storage: Your chat histories and API keys reside exclusively in your browser's localStorage. Clearing your browser data will wipe stored chats and keys. Use caution on shared computers.
