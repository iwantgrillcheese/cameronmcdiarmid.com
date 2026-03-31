# cameronmcdiarmid.com

Personal website for Cameron McDiarmid. Static HTML/CSS/JS — no build step required.

## Deploy to Vercel

### Option 1: Vercel CLI
```bash
npm i -g vercel
vercel --prod
```

### Option 2: GitHub + Vercel UI
1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project → Import Git Repository
3. Select the repo — Vercel auto-detects static HTML, no config needed
4. Add your custom domain: `cameronmcdiarmid.com` in Project Settings → Domains

## Custom Domain Setup
In your domain registrar (e.g. Namecheap, GoDaddy), add:
- `A` record → `76.76.21.21` (Vercel IP)
- `CNAME` for `www` → `cname.vercel-dns.com`

Then add both `cameronmcdiarmid.com` and `www.cameronmcdiarmid.com` in Vercel's domain settings.

## Files
- `index.html` — main page
- `style.css` — all styles
- `script.js` — scroll animations + nav highlight
- `vercel.json` — deployment config + security headers

## Updating content
Everything is plain HTML. Open `index.html`, edit the text, commit, push — Vercel auto-deploys on every push to `main`.

## Things to update before launch
- [ ] Email address in contact section (currently `cam@cameronmcdiarmid.com`)
- [ ] LinkedIn/Twitter/Strava URLs in contact section
- [ ] TrainGPT URL if it changes
- [ ] Work history details (fill in earlier career specifics)
- [ ] Add writing posts when ready (swap placeholder items in `#writing`)
- [ ] Add a favicon (drop `favicon.ico` or `favicon.svg` in root)
