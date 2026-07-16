# AI Component Generator

A React + Vite app that generates UI component code using the Google Gemini API.

## Setup

1. Copy `.env.example` to `.env`
2. Set `VITE_GOOGLE_API_KEY` to your Google Cloud API key
3. Optionally set `VITE_GOOGLE_MODEL=gemini-2.0-flash-001`
4. Run `npm install`
5. Start the app with `npm run dev`

> If you receive a 429 quota error, verify your Google Cloud project's billing and quota settings for `generativelanguage.googleapis.com`.

## Notes

- This app currently sends the API key from the browser.
- For production, route requests through a backend to keep your key secret.
- If your project has no free-tier quota for Gemini, enable billing or use a paid quota.

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
