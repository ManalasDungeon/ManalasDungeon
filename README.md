**🇬🇧 English** · [🇱🇻 Latviešu](README.lv.md)

# Marko Nakari (Mana)

**Software Developer** · Heinola, Finland · Open to roles in Latvia (Vidzeme region or remote)

[🌐 manalasdungeon.lv](https://manalasdungeon.lv) · [✉️ marko.nakari@inbox.lv](mailto:marko.nakari@inbox.lv) · [💼 LinkedIn](https://www.linkedin.com/in/manalainen/) · [🐙 GitHub](https://github.com/ManalasDungeon)

---

## About me

Software developer who graduated from **Vamia** on **1 October 2026**. I have worked at Heinola Library in Finland since 2006, and as a media instructor since April 2025. Alongside library work I have built software that library visitors use.

My strongest area is **PHP/MySQL web development on LAMP and shared hosting** (cPanel, phpMyAdmin, Apache configuration). I also build desktop applications in C#/.NET. I care about secure code, testing and fast, well-indexed websites.

## Work experience

| | |
|---|---|
| **Media Instructor (Mediaohjaaja)** | Heinola Library · 04/2025 – present |
| **Library Clerk (Kirjastovirkailija)** | Heinola Library · 2006 – 2025 |

## Education

| | |
|---|---|
| **Software Developer (Ohjelmistokehittäjä)** | Vamia, remote studies · 2026 |
| **Library Merkonomi (Kirjastomerkonomi)** | Vocational qualification · 1996 |
| **Matriculation examination (Ylioppilas)** | Finnish upper secondary school · 1991 |

## Tech stack

| Area | Technologies |
|---|---|
| Languages | PHP, JavaScript, C#, Kotlin, Python, SQL |
| Web | HTML5, CSS3, Bootstrap 5, vanilla JS |
| Back end & server | Apache (mod_rewrite, .htaccess, caching, gzip), cron, cPanel |
| Databases | MySQL, PDO, phpMyAdmin, MySQL Connector/NET |
| Desktop | .NET WinForms |
| Testing | PHPUnit |
| SEO | Open Graph, schema.org JSON-LD, hreflang, sitemaps |

---

## Featured projects

### 📚 Manalan Kirjasto — library management system

**Live:** [manalasdungeon.lv/verkkokirjasto](https://manalasdungeon.lv/verkkokirjasto/)
**Stack:** PHP · JavaScript · MySQL · C# WinForms

One library system, built twice: as a web application and as a desktop application on the same MySQL database.

**Web version**
- Loans, returns and customer registration, with an automatic return system run by cron
- Security work: SQL injection fixes, PIN hashing with `password_hash()` and `random_int()`, brute-force protection, admin PIN reset, and a fix for a race condition in customer registration
- PHPUnit test suite with 25 test cases using PDO mocks
- Code review that fixed more than 23 issues, including a `GROUP BY` bug in loan queries
- Gothic dark theme with an animated splash screen; documentation written in Word

**Desktop version (C# WinForms)**
- Search-to-lend workflow
- SSL-hardened database connection, typed ListBox objects and an `OperationResult` pattern for error handling

---

### 🌊 Vitrupes Pludmale — tourism website

**Live:** [manalasdungeon.lv/vitrupe](https://manalasdungeon.lv/vitrupe/)
**Stack:** PHP · Bootstrap 5.3 · JavaScript · MySQL · Apache

A tourism website about Vitrupe beach on the Vidzeme coast of Latvia, with a modern visual design based on traditional Latvian colours and woven-band patterns.

- **Three languages** (Latvian, English, Finnish) using PHP language files, with clean `/en/` and `/fi/` URLs via mod_rewrite
- **Performance:** upgraded Bootstrap 4 → 5.3 and removed jQuery, cutting JavaScript from 252 KB to 80 KB; cache busting with `filemtime`, Apache caching and gzip; optimised photos (32.9 MB → 3.4 MB)
- **SEO:** hreflang, a multilingual sitemap, Open Graph and Twitter cards, and schema.org `TouristAttraction` structured data
- **Guestbook with moderation:** CSRF protection, honeypot, rate limiting, safe link rendering, and a bcrypt-protected admin panel where new messages wait for approval
- Image gallery with lightbox, scroll animations and a beach-sound button

---

### 🐦 Lintujen tunnistus — bird identification game

**Live:** [manalasdungeon.lv/birdgame](https://www.manalasdungeon.lv/birdgame/)
**Stack:** PHP · JavaScript · CSS

An educational game built for **"Sula", the library bus in Heinola**, where visitors learn to recognise Finnish birds.

- 14 bird species, each with an info card (scientific name, habitat, fun fact)
- Three languages (Finnish, English, Latvian) with a flag-button language switcher
- Questions shuffled per session, card-based interface designed for the library bus

---

## Languages

| Language | Level |
|---|---|
| Finnish | Native |
| English | Fluent |
| Latvian | Basic |
| Swedish | Basic |

## Contact

- **Email:** marko.nakari@inbox.lv
- **Website:** [manalasdungeon.lv](https://manalasdungeon.lv)
- **LinkedIn:** [linkedin.com/in/manalainen](https://www.linkedin.com/in/manalainen/)
- **GitHub:** [github.com/ManalasDungeon](https://github.com/ManalasDungeon)
- **Location:** Heinola, Finland — open to relocating to Latvia or working remotely
