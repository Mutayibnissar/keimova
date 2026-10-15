# Keimova Study Assistant — secure AI backend

The GitHub Pages frontend is static. **Never put an OpenAI API key in HTML, JavaScript, GitHub Pages, or browser local storage.** This Cloudflare Worker keeps the key in a server-side secret and exposes a small, origin-restricted study endpoint.

## 1. Deploy the Worker

1. Create a Cloudflare account and create a Worker named `keimova-study-api`.
2. Paste `backend/cloudflare-worker.js` into the Worker editor and deploy it.
3. In Worker **Settings → Variables and Secrets**, add:
   - Secret `OPENAI_API_KEY`: your API key.
   - Variable `OPENAI_MODEL`: `gpt-4.1-mini` (or a model available to your API project).
   - Variable `ALLOWED_ORIGINS`: the exact origin serving Keimova, e.g. `https://YOUR-USERNAME.github.io`. Do not include a path or trailing slash. Add other origins comma-separated only if required.
4. Add a Cloudflare rate-limiting rule for the Worker route (start conservatively, for example a small number of POST requests per minute per IP) and review provider usage limits. Origin checks alone are not authentication and can be spoofed by non-browser clients.
5. Test with a non-sensitive question. The endpoint accepts POST JSON at `/study` (or `/`) with `mode`, `topic`, `level`, and optional `context`.

## 2. Connect Keimova

Open the Study Assistant, paste the deployed Worker URL (for example `https://keimova-study-api.YOUR-SUBDOMAIN.workers.dev/study`) into **Connect a private AI backend**, then choose **Save endpoint on this device**. The endpoint is stored only in that browser. Disconnect it to return to guided demo mode.

## Security and limitations

- Keep the API key in Worker secrets only. Never commit it to the repository.
- The Worker uses an exact origin allowlist, request size limits, input validation, a fixed upstream API host, and bounded model output. Add platform-level rate limiting before sharing publicly.
- This starter does not provide user accounts, persistent chat history, retrieval from course documents, or guaranteed abuse prevention. Do not enter confidential, personal, or sensitive information.
- AI answers can be incorrect; verify important claims and calculations with reliable course sources.
- GitHub Pages cannot run the Worker itself. Deploy the backend separately and configure its endpoint before live AI mode can work.

Official references: OpenAI Responses API documentation and Cloudflare Workers documentation.
