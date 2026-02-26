# YouTube Backlink Generator

A lightweight, client-side YouTube backlink generator tool.

This tool generates a list of clickable backlink URLs for any YouTube video and allows submission to multiple web archive services.

No automation. No iframe injection. No background requests.

---

## Features

- Generate backlinks from a YouTube video URL
- Clickable backlink list
- Shuffle templates on load
- Auto-start when URL parameter is present
- Download backlink list (.txt)
- Shareable URL support
- One-click archive submission to:
  - Internet Archive (Wayback Machine)
  - Ghostarchive
  - Archive.today
  - Megalodon.jp
  - Archive.st
- 100% client-side JavaScript
- No backend required

---

## How It Works

1. User enters a YouTube video URL
2. The video ID is extracted
3. Templates are loaded from `youtube-backlink-templates.json`
4. Templates are shuffled
5. The video ID is injected into each template
6. Clickable backlinks are displayed
7. User can download or submit to archive services

---

## Shareable URL Format

The tool supports auto-loading via URL parameter:

```
https://yourdomain.com/?https://www.youtube.com/watch?v=VIDEO_ID
```

When opened:
- The video URL auto-fills
- Backlinks generate automatically

---

## Archive Integration

Archive submission is performed using standard HTML form POST/GET requests to:

- https://web.archive.org/save/
- https://ghostarchive.org/archive2
- https://archive.today/submit/
- https://megalodon.jp/pc/main
- https://archive.st/

No API keys required.

---

## Project Structure
| File/Folder            | Description                                  |
|------------------------|----------------------------------------------|
| [/index.html](https://backlink-generator-tool.github.io/youtube-backlink-generator/index.html)
| [/youtube-backlink-templates.js](https://backlink-generator-tool.github.io/youtube-backlink-generator/youtube-backlink-templates.js)
| [/youtube-backlink-templates.json](https://backlink-generator-tool.github.io/youtube-backlink-generator/youtube-backlink-templates.json)

---

## Deployment

This project can be deployed using:

- GitHub Pages
- Cloudflare Pages
- Netlify
- Vercel
- Any static hosting provider

To deploy with GitHub Pages:

1. Push repository to GitHub
2. Go to Settings → Pages
3. Select branch
4. Save

---

## License

MIT License

---

## Disclaimer

This tool only generates backlink URLs based on templates.
It does not automate traffic, indexing, or ranking manipulation.
Users are responsible for how they use generated URLs.
