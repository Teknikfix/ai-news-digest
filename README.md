# AI News Digest API (local)

Auto-generated daily by the "AI-nyheter dagligen" automation. Read these files
directly from disk - no server or auth needed.

## Files

| File | Content |
|---|---|
| `latest.json` | Full digest: all sections, all groups |
| `index.json` | Metadata, counts and file listing |
| `sections/kimi.json` | Only Kimi |
| `sections/codex.json` | Only Codex |
| `sections/claude.json` | Only Claude |
| `sections/grok.json` | Only Grok |
| `history/YYYY-MM-DD.json` | Daily archive |

## Item shape

```json
{
  "title": "headline or release name",
  "url": "link to source",
  "source": "Hacker News | Google News | GitHub release | npm release | PyPI release | GitHub nytt repo",
  "date": "YYYY-MM-DD HH:MM (UTC)",
  "description": "short summary, may be empty",
  "metric": "points/stars/version, may be empty"
}
```

Top level: `generatedAt`, `lookbackDays`, `sections[]` (each with `id`,
`title`, `groups[]` where group `kind` is `news` / `release` / `community`),
plus `errors[]` listing sources that failed this run.

## Public endpoints (no auth)

| URL | Content |
|---|---|
| https://raw.githubusercontent.com/Teknikfix/ai-news-digest/main/latest.json | Full digest |
| https://raw.githubusercontent.com/Teknikfix/ai-news-digest/main/index.json | Metadata and counts |
| https://raw.githubusercontent.com/Teknikfix/ai-news-digest/main/sections/kimi.json | Only Kimi |
| https://raw.githubusercontent.com/Teknikfix/ai-news-digest/main/sections/codex.json | Only Codex |
| https://raw.githubusercontent.com/Teknikfix/ai-news-digest/main/sections/claude.json | Only Claude |
| https://raw.githubusercontent.com/Teknikfix/ai-news-digest/main/sections/grok.json | Only Grok |
| https://raw.githubusercontent.com/Teknikfix/ai-news-digest/main/history/YYYY-MM-DD.json | Daily archive |

Last updated: 2026-10-18 21:40 UTC
