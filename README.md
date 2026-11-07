# Squeek Aura Checklist

A free, read-only tool for Squeekchain Genesis members. No wallet connection, no transactions, no keys, no backend.

Paste a Sepolia wallet address to see live SQK, power, stake and claimable rewards, tick off Aura badges from the live catalog (saved in your browser), and check the top of the leaderboard.

## What it does

- **Wallet dashboard** — live account data from `https://api.squeekchain.com/v1/accounts/{address}`: claimable SQK, power, stake, token counts.
- **Badge checklist** — live catalog from `https://community.squeekchain.com/v1/community/aura/badges`, grouped by lane (clout / code / holder). Checkboxes persist in localStorage.
- **Profile import** — paste your Genesis referral code, open your public profile JSON at `https://community.squeekchain.com/v1/community/profiles/{code}`, paste the JSON to see Aura, rank, tier and next-tier progress. (The profile endpoint only allows `squeekchain.com` origins, so direct fetch from this page is blocked by CORS — paste is the way.)
- **Leaderboard + stats** — top 10 from `/leaderboard` and totals from `/stats`.

## Hosting

Single static file (`index.html`, ~38 KB). Hosted on GitHub Pages at a custom DuckDNS subdomain, served over HTTPS.

## Data sources

- https://api.squeekchain.com
- https://community.squeekchain.com/v1/community
- https://squeekchain.com/genesis/code

## Squeekchain verification

<!-- The verification line from the Squeekchain project challenge goes here after the project is submitted at https://squeekchain.com/genesis/code. Keep the DNS TXT record, the page tag in index.html, and this line in place — they are rechecked daily. -->
