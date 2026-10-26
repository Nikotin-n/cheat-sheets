# 📞 Phone Number OSINT Cheat Sheet

## 📌 Methodology
1. **Validation & Carrier Lookup:** Identify country code, region, line type (mobile/landline/VoIP), and carrier.
2. **Account Association:** Check linked social media, messengers (Telegram, WhatsApp, Signal, Viber), and apps.
3. **Caller ID & Leaks:** Search public records, caller ID databases, and data breach dumps.
4. **Pivot:** Extract full names, email addresses, or usernames tied to the phone number.

---

## 🛠️ CLI Tools
| Tool | Description | Quick Command |
| :--- | :--- | :--- |
| **PhoneInfoga** | Advanced OSINT scanner for phone numbers | `phoneinfoga scan -n +380XXXXXXXXX` |
| **Ignorant** | Check if phone number is registered on Amazon | `ignorant +380XXXXXXXXX` |
| **Scrappy-PH** | Scrape information from phone lookup resources | `python3 main.py -n +380XXXXXXXXX` |

---

## 🌐 Web Services & Databases
* **NumLookup:** `numlookup.com` (Carrier, location, and owner lookup)
* **EmobileTracker:** `emobiletracker.com` (Free owner name and location trace)
* **Truecaller:** `truecaller.com` (Crowdsourced caller ID search)
* **Sync.ME:** `sync.me` (Social graph & caller identification)
* **FreeCarrierLookup:** `freecarrierlookup.com` (Carrier and SMS gateway info)

---

## 📱 Messengers & Mobile Apps
* **Telegram:** Add number to contacts -> Check profile/avatar via `@username_to_id_bot`.
* **WhatsApp:** Save number or use direct link `https://wa.me/380XXXXXXXXX`.
* **Viber:** Add to contacts to view name, profile picture, and online status.
* **Signal:** Search by number in-app to verify registered user status.

---

## 🎯 Search Operators (Google Dorks)
```text
"+380XXXXXXXXX" OR "0XXXXXXXXX"
"380XXXXXXXXX" filetype:pdf OR filetype:xlsx
site:facebook.com "+380XXXXXXXXX"
site:t.me "+380XXXXXXXXX"
site:viber.com OR site:whatsapp.com "+380XXXXXXXXX"
