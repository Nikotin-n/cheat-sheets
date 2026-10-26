
# 👤 Username Enumeration, Digital Footprinting & Identity Profiling

## 📌 1. Theoretical Framework & Methodology

Username correlation is a core OSINT technique used to track an entity's digital footprint across web platforms, social networks, developer portals, forums, and gaming services. 

Because humans frequently reuse identical or slightly modified handles across multiple platforms due to cognitive bias and personal branding, analyzing username patterns allows analysts to:
* **Map Accounts:** Connect disparate public profiles to a single real-world identity or organization.
* **Identify Tech Stacks:** Uncover developer activity on GitHub, GitLab, DockerHub, or Stack Overflow.
* **Determine Geolocation & Habits:** Analyze timezone activity, language choices, and localized platform presence (e.g., VK, Douban, Reddit).
* **Discover Leaked Metadata:** Find linked email addresses, PII (Personally Identifiable Information), and historic credentials.

---

## 🧭 2. Username Pattern Generation (Handle Permutations)

When a target username is taken or slightly altered on certain platforms, use a systematic permutation matrix to identify potential alt handles:

```text
Target Base Handle: "john_doe"

Permutation Matrix:
├── Prefix Addition:      [sys_john_doe, dev_john_doe, real_john_doe, the_john_doe]
├── Suffix Addition:      [john_doe_dev, john_doe_sec, john_doe_official, john_doe99]
├── Separator Variation:  [john-doe, johndoe, john.doe, john_doe_]
└── Leetspeak / Substitutions: [j0hn_d0e, johnd0e, j0hndoe]
