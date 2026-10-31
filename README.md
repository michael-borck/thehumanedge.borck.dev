# thehumanedge.borck.dev

Landing page for *The Human Edge: Using AI with Judgement* by Michael Borck, and the Curtin Executive Education masterclass of the same name.

Astro 5, plain CSS, deployed to GitHub Pages.

## Local development

```bash
npm install
npm run dev    # http://localhost:4321
npm run build  # ./dist
npm run preview
```

## Structure

```
src/
  pages/index.astro      # The whole page
  styles/global.css      # Cream, dark green, gold palette from the book cover
public/
  CNAME                  # thehumanedge.borck.dev
  cover.png              # Book cover
  favicon.svg
  og.png                 # Social card
  robots.txt
  sitemap.xml
.github/workflows/deploy.yml
```

## Cloudflare DNS

Create one record:

- Type: `CNAME`
- Name: `thehumanedge`
- Target: `michael-borck.github.io`
- Proxy status: DNS only, grey cloud
- TTL: Auto

Do not proxy the record. GitHub Pages needs to issue its own certificate.

## Content status

The book is in manuscript. The masterclass is live at
[the-human-edge](https://michael-borck.github.io/the-human-edge/).

The page links to:

- Conversation, Not Delegation: https://conversationnotdelegation.com
- Books: https://books.borck.education
- Consulting: https://borck.consulting
- borck.dev: https://borck.dev
