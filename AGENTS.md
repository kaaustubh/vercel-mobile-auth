# Vercel Mobile Auth — Agent Memory

## What this is
The OAuth redirect/callback landing pages for **vercel-mobile**'s "Sign in with Vercel"
flow. Vercel redirects here after the user approves; the page hands the auth `code` back
to the app (deep link). Pairs with [vercel-mobile].

## Stack & layout
- Static HTML: `index.html` and `callback/index.html`
- Hosted on GitHub Pages; no build step

## Learnings
- This must stay aligned with the OAuth redirect URI configured in the Vercel app and in
  vercel-mobile's auth code. Changing the callback path here breaks sign-in.
