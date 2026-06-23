# duckduckgo-search — Privacy-friendly web search via Python library

> Full-featured DuckDuckGo search using the `duckduckgo-search` Python package. No API key required. Supports text, news, images, and video search.

[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://github.com/NachaFromMars)

## Overview
duckduckgo-search provides web search capabilities through the `duckduckgo-search` Python library. It requires no API key, respects user privacy (no tracking), and supports four search types: text, news, images, and video. Results include title, URL, and snippet for each entry, making them easy to parse and feed into further processing.

## Features
- **Text search** — general web results
- **News search** — current events
- **Image search** — image results with metadata
- **Video search** — video results
- **No API key** — free and private
- **Returns** — title, href (URL), body (snippet) per result

## Usage / Quick Start
```bash
pip install duckduckgo-search
# or
uv pip install duckduckgo-search
```
```python
from duckduckgo_search import DDGS

with DDGS() as ddgs:
    results = list(ddgs.text("your query", max_results=5))
    for r in results:
        print(r["title"], r["href"])
```

## Trigger Keywords (OpenClaw)
search web, DuckDuckGo, find information, current events, web search, no API search

## Related Skills
- [ddg-web-search](https://github.com/NachaFromMars/ddg-web-search) — zero-install alternative using web_fetch

---
Part of the [NachaFromMars](https://github.com/NachaFromMars) OpenClaw skill ecosystem.
