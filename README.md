# Oxford Spoken English Classes: landing page

Single-file landing page for the Meta ads (English). Open `index.html` to preview. No build step.

## Before going live (edit the CONFIG block at the top of index.html)
- `whatsapp`: Oxford WhatsApp Business number, format `91XXXXXXXXXX`
- `slots`: the two real group demo slots
- `demoMode`: e.g. "Zoom" or "At the Radha Nagar class"
- `seatsLeft`: real number or 0 to hide
- `showGoogleRating`: set `true` only after 4.9 stars / 691 reviews is verified on Google
- `videoSrc`: student testimonial video (mp4); empty hides the block
- `pixelId`: Meta Pixel ID

## Behaviour
- Form opens WhatsApp with a pre-filled booking message (name, goal, slot, mobile, ad source from `utm_campaign` or `utm_source`).
- Meta Pixel events: PageView, Lead (form submit), CTAClick (each button).
- No prices on the page by design. The page is `noindex`; remove the robots meta tag only if you want it in search.

## Deploy
Static file. Drop it on Vercel, Netlify or Hostinger as `index.html`.
