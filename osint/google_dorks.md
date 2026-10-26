# 🔎 Advanced Google Dorking & Reconnaissance Methodology

## 📌 Introduction & Methodology
Google Dorking (or Google Hacking) is a passive reconnaissance technique based on leveraging advanced search engine operators to uncover sensitive data, hidden directories, unprotected configuration files, and vulnerable endpoints without directly interacting with the target infrastructure (i.e., without sending requests to the target's web server).

---

## 🛠️ Core Syntax & Operators

| Operator | Purpose & Description | Usage Example |
| :--- | :--- | :--- |
| `site:` | Restricts search results to a specific domain or subdomain. | `site:subdomain.example.com` |
| `filetype:` / `ext:` | Filters results by specific file extension (PDF, DOCX, SQL, ENV, etc.). | `ext:log OR ext:env` |
| `inurl:` | Searches for a specific string within the URL path. | `inurl:api/v1` |
| `intitle:` | Finds matches within the HTML `<title>` tag of a webpage. | `intitle:"Dashboard"` |
| `intext:` / `allintext:` | Searches for specific keywords within the body text of a webpage. | `intext:"DB_PASSWORD"` |
| `cache:` | Displays Google's cached version of a webpage (useful if the site is offline). | `cache:example.com` |

---

## 🚀 Professional Dorks for Vulnerability & Leak Discovery

### 1. Identifying Sensitive Data & Configuration Leaks (Information Disclosure)
Search for environment configuration files, hardcoded credentials, and log files indexed by accident:
```text
site:example.com (ext:env OR ext:yaml OR ext:json OR ext:xml OR ext:ini) "DB_PASSWORD"
