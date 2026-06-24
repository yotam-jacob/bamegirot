# במגירות — TODO

## Before launch

- [ ] Review the "קצת עליי" paragraph — confirm Lior is happy with the wording

## Connect bamegirot.com domain (Wix → Vercel)

**Step 1 — Add domain in Vercel**
- [ ] Go to vercel.com → your project (mom-antiques) → Settings → Domains
- [ ] Add `bamegirot.com` → Vercel will show you the DNS records to copy

**Step 2 — Add DNS records in Wix**
- [ ] Log in to wix.com → Domains → Manage next to bamegirot.com
- [ ] Go to Advanced → DNS Records
- [ ] Add an **A record**: Host = `@` · Value = `76.76.21.21` (Vercel's IP)
- [ ] Add a **CNAME record**: Host = `www` · Value = `cname.vercel-dns.com`
- [ ] Delete any existing A record pointing to Wix (if one exists for `@`)
- [ ] Save

**Step 3 — Wait & verify**
- [ ] Wait up to 48 hours for DNS to propagate (usually under 1 hour)
- [ ] Visit https://bamegirot.com — should load the site with a green padlock
- [ ] Visit https://www.bamegirot.com — should redirect to the same site

**Step 4 — Cleanup**
- [ ] Update the OG image meta tag in index.html if it doesn't already point to bamegirot.com (it already does — just verify it loads)
- [ ] Run `~/.npm-global/bin/vercel --prod --yes` to redeploy with the live domain active

## After launch

- [ ] Add negative keywords to Google Ads: `פינוי`, `סוחר עתיקות`, `וינטג'`, `שמאי`, `גמולב`, `buy antique items` (~₪238/month waste)

## Done

- [x] Business name → במגירות
- [x] WhatsApp number → 972523321045
- [x] Years of experience → 5+
- [x] Families helped → עשרות+
- [x] Domain → https://www.bamegirot.com/
- [x] Hero cover image — full-bleed with text overlay
- [x] 3 real testimonials (מיכל, ליאת, יעל)
- [x] Portrait photo → images/portrait.jpg (live in "קצת עליי" section)
- [x] 21 item photos → sold items gallery section
- [x] Removed all "free evaluation" / "חינם" references
- [x] Removed all silver / "כסף ישן" references
- [x] Voice changed to first-person (ליאור) throughout
- [x] Mobile optimized — floating WhatsApp button, responsive gallery, full-width CTAs
