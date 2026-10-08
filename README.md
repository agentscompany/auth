# auth.agentscompany.ai

Static sign-in pages for the Agents Company app, served by GitHub Pages.

Some providers (Mercado Livre, Figma) only accept a fixed HTTPS redirect URI. Their sign-in lands on a page here, which hands the result to the Agents Company app running on the user's own computer (`http://127.0.0.1:<port>/callback`; the port travels in `state`). The pages run only in the user's browser: no server, no storage, no third-party scripts. The authorization code is useless without the PKCE verifier that only the app holds.

- `mercadolivre.html` — Mercado Livre (`https://auth.agentscompany.ai/mercadolivre`)
- `figma.html` — Figma (`https://auth.agentscompany.ai/figma`)
