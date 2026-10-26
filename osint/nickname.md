# 🕵️‍♂️ Username OSINT Cheat Sheet

## 📌 Methodology
1. **Enumeration:** Search across platforms using automated scanners.
2. **Permutation:** Test variations (prefixes, suffixes, numbers, separators).
3. **Verification:** Cross-reference profile pictures, bios, external links, and unique account IDs.

---

## 🛠️ CLI Tools
| Tool | Description | Quick Command |
| :--- | :--- | :--- |
| **Sherlock** | Search across 400+ platforms | `python3 sherlock username` |
| **Maigret** | Scan 3000+ sites & collect metadata | `maigret username --html` |
| **WhatsMyName** | Fast search using WMN framework | `whatsmyname -u username` |
| **Blackbird** | Async search engine for handles | `python3 blackbird.py -u username` |

---

## 🌐 Web Services
* **WhatsMyName App:** `whatsmyname.app`
* **Namechk:** `namechk.com`
* **KnowEm:** `knowem.com`
* **Social Searcher:** `social-searcher.com`

---

## 🎯 Search Operators (Google Dorks)
```text
"username"
site:github.com "username"
site:twitter.com OR site:x.com "username"
inurl:username
site:t.me/username
site:[reddit.com/user/username](https://reddit.com/user/username)
