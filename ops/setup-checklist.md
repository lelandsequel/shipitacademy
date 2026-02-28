# Setup Checklist

Complete everything below by **Thursday evening** before the weekend. If you arrive Saturday without this done, you will fall behind.

---

## Development Environment

### All Participants
- [ ] Laptop with at least 8GB RAM, working charger, and a code editor installed
- [ ] Terminal/shell configured and working
- [ ] Git installed and configured (`git --version` returns a version number)
- [ ] GitHub account created and SSH key or token configured
- [ ] Node.js 18+ or Python 3.10+ installed (depending on your build language)
- [ ] Package manager working (`npm` or `pip`)

### Ship Systems Track (additional)
- [ ] Code editor with extensions for your language (VS Code recommended)
- [ ] Deployment platform account created (Vercel, Railway, Fly.io, or Render — pick one)
- [ ] Deployment CLI installed (e.g., `vercel`, `railway`, `flyctl`)
- [ ] Screen recording tool installed (Loom, QuickTime, or OBS)

### Leverage Systems Track (additional)
- [ ] Access to your actual work files/data for the leverage exercise
- [ ] Any integration tools you plan to use (Notion API, Google Docs API, Slack API, etc.)
- [ ] A prospect in mind for the outreach module (someone you can actually message)

---

## API Keys & Accounts

- [ ] AI model provider account and API key (at least one):
  - Anthropic (Claude): https://console.anthropic.com
  - OpenAI: https://platform.openai.com
- [ ] API key tested — run a simple API call and confirm you get a response
- [ ] Billing configured on your API account (free tiers may hit limits during the build)
- [ ] `.env.example` file understood — never commit API keys to a repo

---

## Repository Access

- [ ] Weekend repo forked or cloned (link provided in your confirmation email)
- [ ] Repo builds and runs locally without errors
- [ ] You can push commits to your fork

---

## Communication

- [ ] Discord account created
- [ ] Joined the Operator Foundry Discord server (invite link in confirmation email)
- [ ] Introduce yourself in the #introductions channel (name, what you do, what you're building)
- [ ] Notifications enabled for the weekend channel

---

## Optional but Recommended

- [ ] Second monitor or tablet for reference material
- [ ] Headphones for focused build blocks
- [ ] Water bottle and snacks (you won't want to leave during build blocks)
- [ ] Phone on silent or do-not-disturb for Saturday and Sunday

---

## Verification

Run these commands to confirm your setup:

```bash
# Git
git --version

# Node.js (if using)
node --version
npm --version

# Python (if using)
python3 --version
pip --version

# API test (example with curl — replace with your key)
curl https://api.anthropic.com/v1/messages \
  -H "x-api-key: $ANTHROPIC_API_KEY" \
  -H "content-type: application/json" \
  -H "anthropic-version: 2023-06-01" \
  -d '{"model":"claude-haiku-4-5-20251001","max_tokens":50,"messages":[{"role":"user","content":"Say hello"}]}'
```

If any command fails, fix it before Saturday or ask in the Discord #setup-help channel.

---

**Questions?** Post in Discord #setup-help. Do not wait until Saturday morning.
