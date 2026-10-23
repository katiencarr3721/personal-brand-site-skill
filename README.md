# Personal Brand Site Builder (Claude skill) · v3.0

A Claude skill that turns your resume, LinkedIn, and a headshot into a polished, single-page personal site, with optional AI features (a chat agent that answers questions about your background and a personalized pitch generator). It interviews you first, builds the site, checks every claim with you, and walks you through deploying it.

It's the skill that built [katiencarr.ai](https://katiencarr.ai).

## What it does

- **Guided intake:** a short interview covering your goal, materials, brand, the hardest room you've proven yourself in, and which sections you want.
- **Safe-list first:** you decide which facts and numbers are public before any copy is written. Hard numbers or qualitative outcomes only: your choice.
- **Builds the site:** one HTML file, mobile-first, accessible, with production-proven sections: animated proof, case studies, speaking, an operating-principles console, a scroll-driven career journey, a layered About, a skill map that makes the case for a non-traditional path, and intent-based contact.
- **Optional AI features:** a chat agent and a pitch generator on serverless functions, with moderation, PII scrubbing, rate and cost caps, and counts-only analytics.
- **Quiet job search mode:** the public site reads as a practitioner sharing their work, and the pitch tools and resume sit behind a server-side password.
- **Guided deployment:** a private preview first, then Netlify, Vercel, or GitHub Pages, tailored to your comfort level.

## Install

**Claude desktop app (Cowork):** download [`dist/personal-brand-site.skill`](dist/personal-brand-site.skill), open Cowork, and upload the file to install it. Then say *"build me a personal website"*.

**Claude Code:** copy the `personal-brand-site/` folder into your skills directory (for example `~/.claude/skills/personal-brand-site/`).

## What you'll need

- A resume or LinkedIn profile, plus a professional headshot
- About an hour, start to finish (interview, review, deploy)
- A free hosting account (Netlify recommended if you want the AI features)
- A Claude API key from [console.anthropic.com](https://console.anthropic.com) if you want the AI features

## Repo layout

```
personal-brand-site/SKILL.md     # the skill itself (source of truth)
dist/personal-brand-site.skill   # packaged, installable build of the folder above
LICENSE                          # MIT
```

To rebuild the package after editing `SKILL.md`:

```bash
zip -X -r dist/personal-brand-site.skill personal-brand-site
```

## License

MIT: free to use, copy, adapt, and share, as long as the copyright notice stays with it. See [`LICENSE`](LICENSE).

## Version

v3.0 (2026-10-23). Full history is at the bottom of `SKILL.md`.

---

Built by [Katie Carr](https://katiencarr.ai). Try it live, and build your own AI skill in the Workshop at [katiencarr.ai/#workshop](https://katiencarr.ai/#workshop).
