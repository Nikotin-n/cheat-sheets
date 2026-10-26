# 🔎 Advanced Google Dorking & Reconnaissance Methodology

## 📌 Introduction & Theoretical Framework
Google Dorking (Google Hacking) is a fundamental passive reconnaissance methodology. It leverages structural search operators to identify exposed sensitive data, misconfigured security headers, public backup files, and unlinked administrative panels indexed by search engine crawlers. Because all queries are processed by Google's infrastructure, this process remains entirely passive and undetectable by the target's direct server logs.

---

## 🛠️ Core Syntax & Operator Reference

| Operator | Syntax Format | Operational Purpose |
| :--- | :--- | :--- |
| `site:` | `site:example.com` | Restricts search scope exclusively to the specified domain or TLD. |
| `filetype:` / `ext:` | `ext:env` / `filetype:pdf` | Filters results by file extension (e.g., configuration, archives, documents). |
| `inurl:` | `inurl:api/v1` | Identifies specific subpaths, directories, or parameters within the URL string. |
| `intitle:` | `intitle:"Index of"` | Matches specific strings within the HTML `<title>` tag of indexed pages. |
| `intext:` | `intext:"DB_PASSWORD"` | Searches for target strings anywhere within the rendered text body of the page. |
| `cache:` | `cache:example.com` | Displays Google’s cached snapshot of a page (useful for offline/removed pages). |

---

## 🚀 Advanced Google Dork Scenarios & Queries

### 1. Information Disclosure & Sensitive Configuration Files
Uncovering environment configuration files, database credentials, and error log dumps:
```text
site:example.com (ext:env OR ext:yaml OR ext:ini OR ext:json OR ext:xml) "DB_PASSWORD"
