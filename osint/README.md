# 🔎 OSINT & Open-Source Intelligence Methodology

## 📌 Overview & Core Concepts
Open Source Intelligence (OSINT) refers to the collection, analysis, and utilization of information derived from public, open sources. In cybersecurity, OSINT is the foundational phase of both offensive assessments (Reconnaissance) and defensive threat intelligence (Threat Intel).

This section serves as a dedicated repository for **OSINT search cheat sheets, methodology guides, and practical lookup tools**. It is designed to document systematic techniques and workflows used to map digital footprints, verify identities, and uncover potential security risks without triggering active alerts on target infrastructure.

---

## 🧭 Key Methodological Pillars

This knowledge base covers the following core operational areas of OSINT:

### 1. Passive Reconnaissance & Search Cheat Sheets
* **Definition:** Collecting data about a target organization, domain, or individual using open search channels without direct network interaction.
* **Content & Guides:** Structured search queries, Google Dorking operators, index lookup patterns, and quick-reference guides for finding exposed data.
* **Application:** Safely identifying exposed configuration files, subdomains, and leaked credentials.

### 2. Digital Footprinting & Account Lookup Tools
* **Definition:** Tracking the digital presence of individuals or entities across various web platforms and services.
* **Content & Tools:** Overview of tools and techniques for username enumeration, cross-platform account correlation, and public data lookup utilities.

### 3. Geolocation & Imagery Analysis
* **Definition:** Extracting intelligence from visual media (photos, videos, architectural features).
* **Key Techniques:** Analyzing EXIF metadata, identifying landmarks, cross-referencing shadow angles, and using satellite/street-view lookup tools for verification.

---

## 🛠️ Documentation & Search Cheat Sheets

Below is the comprehensive collection of OSINT methodologies, search cheat sheets, and tool references available in this repository:

### 🔍 Search Engines & Passive Reconnaissance
* 📑 **[Google Dorking Methodology](./google_dorks.md):** Advanced search operators (`site:`, `ext:`, `inurl:`, `intitle:`) for identifying sensitive files, configuration leaks, and exposed admin portals.
* 📑 **[Alternative Search Engines & Indexing](./alt_search_dorks.md):** Search dorks and methodology for DuckDuckGo, Bing, Yandex, and Shodan queries.
* 📑 **[Wayback Machine & Web Archives](./web_archives_recon.md):** Techniques for recovering deleted web pages, legacy sensitive parameters, and historic site architecture.

### 👤 Identity, Username & Social Footprinting
* 📑 **[Username Enumeration & Profiling](./username_recon.md):** Cross-platform username tracking methodology, API lookup techniques, and tool usage (Sherlock, Maigret).
* 📑 **[Email & Breach Data Investigation](./email_breach_recon.md):** Querying breach databases, OSINT email verification, and identifying linked accounts via open APIs.
* 📑 **[Social Media Intelligence (SOCMINT)](./socmint_guide.md):** Workflow for mapping public social profiles, metadata extraction, and connection analysis.

### 🌐 Infrastructure & Domain Intelligence
* 📑 **[Domain & Subdomain Enumeration](./domain_subdomain_enum.md):** Certificate Transparency logs (`crt.sh`), DNS record auditing, and passive subdomain discovery workflow.
* 📑 **[IP & Infrastructure Mapping](./ip_infrastructure_recon.md):** ASN lookups, WHOIS historical records, reverse IP tracking, and Shodan/Censys query reference.

### 📸 Media, Metadata & Geolocation
* 📑 **[EXIF Metadata Extraction](./exif_metadata_recon.md):** Command-line tools (`exiftool`), image forensic techniques, and extracting geolocation coordinates from media files.
* 📑 **[Geolocation & Imagery Analysis](./geolocation_cheatsheet.md):** Landmark identification, sun/shadow angle tools, and satellite imagery cross-referencing guide.

### 🛠️ Toolkits & Resources
* 📑 **[OSINT Tools & Lookup Services Catalog](./osint_tools_catalog.md):** A curated index of open-source CLI utilities, web-based lookup tools, and specialized investigation frameworks.

---

## ⚖️ Legal & Ethical Boundaries
All cheat sheets, tools, and techniques documented in this repository are strictly intended for **authorized security testing, educational purposes, and defensive research**. Always adhere to legal frameworks and the rules of engagement (RoE) during any security assessment.
