
# 🔎 Alternative Search Engines & Passive Indexing Dorks

## 📌 Overview
While Google is the primary engine for passive reconnaissance, alternative search engines (Bing, DuckDuckGo, Yandex) and specialized scanners (Shodan) index web assets differently. Using multi-engine dorking uncovers hidden endpoints, forgotten staging environments, and legacy parameters missed by Google.

---

## 🌐 1. Bing & DuckDuckGo Advanced Operators

Bing and DuckDuckGo share similar syntax and are exceptionally useful for mapping IP ranges and identifying shared hosting environments.

| Operator | Purpose | Example |
| :--- | :--- | :--- |
| `ip:` | Finds all websites hosted on a specific IPv4 address (Bing only). | `ip:192.0.2.45` |
| `contains:` | Searches for pages linking to specific file types or keywords. | `site:example.com contains:pdf` |
| `filetype:` | Filters by file extension. | `site:example.com filetype:conf` |
| `domain:` | Restricts search to a specific domain hierarchy. | `domain:example.com` |

### 🚀 Practical Search Workflows
```text
# Discover co-hosted domains on a target IP (Bing)
ip:192.0.2.45 site:org

# Find exposed API endpoints or JSON files on DuckDuckGo
site:example.com filetype:json inurl:api
