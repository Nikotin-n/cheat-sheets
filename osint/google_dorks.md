# 🔍 Detailed Google Dorks (GHDB) Cheat Sheet for OSINT

Google Dorking (Google Hacking) is the use of advanced Google search operators to discover hidden information, vulnerabilities, data leaks, open configuration files, and unsecured servers.

---

## 🛠️ 1. Basic and Advanced Google Operators

| Operator | Purpose | Example |
| :--- | :--- | :--- |
| `site:` | Search exclusively within a specified domain or domain zone | `site:gov.ua`, `site:target.com` |
| `filetype:` / `ext:` | Search for files of a specific extension | `filetype:pdf`, `ext:php`, `ext:log` |
| `inurl:` | Search for a specified word in the URL address | `inurl:admin`, `inurl:api` |
| `allinurl:` | All specified words must be present in the URL | `allinurl:etc passwd` |
| `intitle:` | Search for a word in the page title (`<title>`) | `intitle:"Index of"`, `intitle:"Dashboard"` |
| `allintitle:` | All specified words must be present in the page title | `allintitle:restricted access login` |
| `intext:` | Search for a word directly in the page text | `intext:"DB_PASSWORD"` |
| `allintext:` | All specified words must be present in the page text | `allintitle:password admin credentials` |
| `cache:` | View the last saved version of a page in Google cache | `cache:target.com` |
| `related:` | Search for sites with similar topics or structure | `related:target.com` |
| `link:` | Search for pages that link to a specified address | `link:target.com` |

---

## ⚙️ 2. Logical Operators and Syntax Symbols

- **`"..."` (Exact Match):** Searches for a phrase in the exact sequence.
  * `site:target.com "confidential document"`
- **`OR` / `|` (Logical OR):** Searches for at least one of the words (must be capitalized).
  * `site:target.com (filetype:pdf OR filetype:docx)`
- **`AND` (Logical AND):** Requires both conditions to be met (Google applies this by default).
  * `site:target.com intext:admin AND intext:password`
- **`-` (Exclusion / Minus):** Hides results containing specified words or subdomains.
  * `site:target.com -site:www.target.com` *(subdomain discovery)*
- **`*` (Wildcard / Mask):** Replaces one or more arbitrary words or characters.
  * `site:target.com inurl:api/*/v1`
- **`( )` (Grouping):** Combines multiple operators for complex logical conditions.
  * `site:target.com (inurl:admin OR inurl:login) filetype:php`

---

## 🎯 3. Ready-to-Use Practical Dorks by Category

### 🌐 Finding Hidden Subdomains
```text
site:target.com -www.target.com
site:*.target.com -site:[www.target.com](https://www.target.com)
site:target.com -inurl:www -inurl:mail
