# AI Companion Studio

A browser-based AI companion with an editable character profile, chat history, and a server route that can talk to Gemini.

## What it does

- Lets you name the companion and define her species and personality.
- Stores the conversation locally in the browser.
- Calls Gemini from the server when `GEMINI_API_KEY` is set.
- Falls back to a local conversational response when no API key is available.

## Setup

1. Install dependencies:

```bash
npm install
```

2. Create a local environment file from `.env.example` and set your key:

```bash
GEMINI_API_KEY=your_key_here
```

3. Run the app:

```bash
npm run dev
```

4. Open the local URL shown by Next.js.

## Scripts

- `npm run dev` starts the development server.
- `npm run build` creates a production build.
- `npm run start` runs the production server.
- `npm run lint` checks the project with ESLint.

## Notes

- The companion defaults to Mira, a lunar fox with a warm, teasing personality.
- You can change the profile in the UI at any time.
- The Gemini route uses the official REST endpoint directly, so no extra SDK is required.
