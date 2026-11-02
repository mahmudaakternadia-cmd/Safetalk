**SafeTalk** is a real-time group chat application built to make online conversations safer. It allows users to join a chat room, send messages instantly, and automatically filter harmful or abusive content before it reaches other participants. The project combines a Python WebSocket backend with Google authentication and moderation tools to block profanity, toxic language, spam-like behavior, and repeated unsafe activity. It is built for environments where trust, moderation, and community safety are priorities.

**Key features:**
1. Google authentication for secure user login
2. Real-time group messaging using WebSockets
3. Profanity detection with better_profanity
4. Toxicity moderation using Hugging Face API
5. AI-powered safety checks for chat prompts
6. Rate limiting and automatic bans for spam or repeated abuse
7. Logging of flagged or unsafe messages for monitoring
8. Live user presence and chat updates

**Technology stack:**
1. Python
2. WebSockets
3. Google OAuth / Google Auth
4. OpenAI API
5. Hugging Face inference API
6. better_profanity library
7. JavaScript, HTML, and CSS for front-end interaction

This repository focuses on the backend logic and moderation system for SafeTalk, with real-time messaging and safety enforcement at its core. The main logic is implemented in server.py, which handles chat communication, user authentication, moderation checks, and server-side enforcement of safety rules. It includes real-time chat handling, Google-based authentication, profanity and toxicity moderation, spam prevention, and user banning for repeated violations.

**How it works:**
A user signs in using a Google account. The chat server verifies the user Messages are checked for profanity and toxicity Unsafe content is blocked and logged Repeated violations can lead to temporary or permanent bans. The app keeps a live list of active users and broadcasts messages to everyone in the chat
