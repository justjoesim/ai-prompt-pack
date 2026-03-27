# The Ultimate AI Prompt Pack

100 ready-to-use AI prompts for professionals across 8 categories: marketing, content creation, dev, startups, coaching, health & wellness, real estate, and design.

## Project Structure

```
├── content/          # 100 prompts (markdown source, 8 category files)
├── src/              # Landing page (HTML/CSS)
├── scripts/          # PDF + prompt export scripts
├── dist/             # Generated PDF + individual prompt .md files
├── promo/            # Promotional content drafts
└── tests/            # Test files
```

## Setup

```bash
npm install
```

## Build Everything

```bash
npm run build
```

This generates:
- `dist/ai-coding-prompt-pack.pdf` — the full PDF product
- `dist/prompts/` — 100 individual `.md` files organized by category

## Build Individually

```bash
npm run build:pdf      # PDF only
npm run build:prompts  # Individual .md files only
```

## Serve the Landing Page Locally

```bash
npm run serve
```

Then open http://localhost:3456

## Deployment

The landing page auto-deploys to GitHub Pages on every push to `main`.

Enable GitHub Pages in your repo settings:
- Go to Settings → Pages
- Source: GitHub Actions

Your live URL will be: `https://[your-username].github.io/[repo-name]/`

## User Action Checklist

Before going live, complete these steps manually:

- [ ] Create a Gumroad account at https://gumroad.com
- [ ] Connect payment method (PayPal or bank account) in Gumroad settings
- [ ] Build: `npm run build`
- [ ] Upload `dist/ai-coding-prompt-pack.pdf` to Gumroad, set price to $5
- [ ] Optionally zip `dist/prompts/` and add as a bonus download on Gumroad
- [ ] Copy your Gumroad product URL
- [ ] Replace `GUMROAD_URL_HERE` in `src/index.html` with your real Gumroad URL
- [ ] Push to `main` to trigger redeployment
- [ ] Replace `LANDING_PAGE_URL_HERE` in `promo/*.md` with your live GitHub Pages URL
- [ ] Post `promo/reddit-chatgpt.md` to r/ChatGPT or r/artificial
- [ ] Post `promo/reddit-programming.md` to r/Entrepreneur or r/smallbusiness
- [ ] Post `promo/twitter-thread.md` as a thread on Twitter/X
