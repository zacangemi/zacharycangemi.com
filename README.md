# zacharycangemi.com

Source for [zacharycangemi.com](https://zacharycangemi.com) — Zachary Cangemi's personal portfolio site.

A landing page for the rest of the work: projects, hardware builds, writing, and how to reach me.

- **Live site:** https://zacharycangemi.com
- **Blog (separate):** https://blog.zacharycangemi.com

---

## Stack

Vanilla HTML, CSS, and JavaScript. No build step, no framework, no bundler. Static files served as-is via GitHub Pages with a custom domain (`CNAME` → Route 53 DNS pointing at GitHub Pages). Loads fast on any connection.

## Structure

| File | Purpose |
|---|---|
| `index.html` | Home |
| `about.html` | Bio |
| `skills.html` | Skill grid |
| `portfolio.html` | Featured projects (cards) |
| `blog.html` | Index that links out to blog.zacharycangemi.com |
| `contact.html` | Contact form (Formspree) + social links |
| `404.html` | Custom not-found page |
| `rickroll.html` | Easter egg |
| `css/style.css` | All styles |
| `CNAME` | Custom-domain config for GitHub Pages |
| `sitemap.xml`, `robots.txt` | SEO |

## Featured projects (in portfolio.html order, newest first)

- [`owning-your-agent`](https://github.com/zacangemi/owning-your-agent) — local agentic work with Hermes Agent on dual RTX 3090s (Qwen3.5-27B + GLM-4.7-Flash at 96K context).
- [`local-llm-infrastructure`](https://github.com/zacangemi/local-llm-infrastructure) — the dual RTX 3090 build that hosts the inference stack (48 GB VRAM).
- [`melange`](https://github.com/zacangemi/melange) — Apple Silicon LLM memory profiler in Rust.
- This repo ([`zacharycangemi.com`](https://github.com/zacangemi/zacharycangemi.com)) — the site itself.

## Local development

No build required. From the repo root, any of these works:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
npx serve .                   # if you have Node installed
open index.html               # or just open files directly in a browser
```

## Deployment

Pushes to `main` are auto-published by GitHub Pages. The custom domain is wired via the `CNAME` file at the repo root plus Route 53 records pointing `zacharycangemi.com` at `zacangemi.github.io`.

## License

MIT for the source code (HTML, CSS, JS). Image and surfboard graphic assets are under their respective licenses — see `css/` for vendor licenses (e.g. `License for Surfing File from mrbrownjeremy.pdf`).

## Contact

[zacharycangemi.com/contact.html](https://zacharycangemi.com/contact.html) · [GitHub](https://github.com/zacangemi) · [LinkedIn](https://www.linkedin.com/in/zacharycangemi/)
