# Module 08: Deploy

## Ship Systems Weekend — Sunday, 1:00 PM

---

## Objective
Deploy your system to a live URL. When this module is done, anyone with the link can use your system. No "it works on my machine."

## Duration
90 minutes

---

## Facilitator Guide

### Frame (5 min)
> "If it's not deployed, it's not shipped. This is the module where your project goes from a local script to a live system. Pick a platform, configure it, and get a URL."

### Platform Selection (10 min)

| Platform | Best For | Free Tier | Deploy Time |
|----------|----------|-----------|-------------|
| **Vercel** | Next.js, static sites, serverless functions | Yes | ~2 min |
| **Railway** | Full-stack apps, APIs, background workers | Yes (trial) | ~5 min |
| **Fly.io** | Docker containers, global deployment | Yes | ~5 min |
| **Render** | Web services, APIs, static sites | Yes | ~5 min |
| **Replit** | Quick deploys, any language | Yes | ~1 min |

For CLI-only systems: deploy as an API endpoint. The interface module should have given you something deployable. If not, wrap your agent in a minimal API server now.

### Build Block (65 min)

**Step 1: Platform Setup (15 min)**
- Create account (if needed)
- Install CLI tool or connect GitHub repo
- Configure project settings

**Step 2: Environment Configuration (15 min)**
- Set all environment variables on the platform
- Confirm API keys are configured (never commit secrets)
- Set any platform-specific config (build commands, start commands, ports)

**Step 3: Deploy (15 min)**
- Push to deploy (or trigger manual deploy)
- Watch build logs for errors
- Fix any build/deploy issues

**Step 4: Verify (20 min)**
- Open the live URL
- Run through the core flow with real input
- Confirm output matches local behavior
- Test from a different device or incognito window
- Run eval suite against the deployed version (if possible)

### Troubleshooting Session (10 min)
> "Who has a live URL? Raise your hand."

For those who don't:
- What error are you seeing?
- Is it a build error or a runtime error?
- Pair with someone who's deployed to debug

---

## Participant Checklist

- [ ] Platform account created
- [ ] Project connected (via CLI or GitHub)
- [ ] All environment variables set on the platform
- [ ] Build succeeds
- [ ] System is accessible at a live URL
- [ ] Core flow works on the deployed version
- [ ] URL added to README
- [ ] Code committed and pushed

### Deployment Record

**Platform:** ___
**Live URL:** ___
**Deploy method:** ___ (GitHub auto-deploy / CLI push / manual)
**Environment variables configured:** Yes / No
**Core flow verified on live:** Yes / No

---

## Common Deploy Issues

| Issue | Platform | Fix |
|-------|----------|-----|
| Build fails | All | Check build logs, confirm dependencies are in package.json/requirements.txt |
| Missing env vars | All | Platform dashboard > Environment Variables, set each one |
| Port mismatch | Railway, Fly | Use `PORT` env var, don't hardcode port numbers |
| Timeout on AI calls | Vercel | Use serverless function with extended timeout, or switch to Railway |
| Cold start too slow | Vercel, Render | Expected on free tier. Note it in your demo. |

---

## Artifact
Each participant: live deployed system accessible via URL.
