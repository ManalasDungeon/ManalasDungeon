**🇬🇧 English** · [🇱🇻 Latviešu](README.lv.md)

# Marko Nakari (Mana)

**Software developer** · Heinola, Finland · Looking for work in Latvia — Riga, Vidzeme or remote

[🌐 manalasdungeon.lv](https://manalasdungeon.lv) · [📁 Portfolio](https://manalasdungeon.lv/portfolio.php?lang=en) · [🔗 Links](https://manalasdungeon.lv/linkit?lang=en) · [✉️ marko.nakari@inbox.lv](mailto:marko.nakari@inbox.lv) · [💼 LinkedIn](https://www.linkedin.com/in/manalainen/) · [🐙 GitHub](https://github.com/ManalasDungeon)

---

## About me

Software developer, graduated from **Vamia** on 1 October 2026. I have worked at Heinola library in Finland since 2006, and as a media instructor since April 2025. Alongside my library work I have built software that the library’s visitors use.

My strongest area is **PHP/MySQL web development in LAMP environments and on shared hosting** (cPanel, phpMyAdmin, Apache configuration). I also build desktop applications with C#/.NET. I care about secure code, testing and fast, well-indexed websites.

## Work experience

| | |
|---|---|
| **Media instructor (Mediaohjaaja)** | Heinola library · 04/2025 – present |
| **Library clerk (Kirjastovirkailija)** | Heinola library · 2006 – 2025 |

## Education

| | |
|---|---|
| **Software developer (Ohjelmistokehittäjä)** | Vamia, remote studies · 2026 |
| **Library merkonom (Kirjastomerkonomi)** | Vocational qualification · 1996 |
| **Matriculation examination (Ylioppilas)** | Finnish upper secondary school · 1991 |

## Tech stack

| Area | Technologies |
|---|---|
| Programming languages | PHP, JavaScript, C#, Kotlin, Python, SQL |
| Web | HTML5, CSS3, Bootstrap 5, vanilla JS |
| Server | Apache / LiteSpeed (mod_rewrite, .htaccess, caching, gzip), cron, cPanel |
| Databases | MySQL, PDO, phpMyAdmin, MySQL Connector/NET |
| Security | WebAuthn / FIDO2 (passkeys), OpenSSL, OWASP Top 10 |
| Desktop | .NET WinForms |
| Testing | PHPUnit, Playwright |
| Images | Python (Pillow) |
| SEO | Open Graph, schema.org JSON-LD, hreflang, sitemaps |

---

## Main projects

### 🔐 manalasdungeon.lv — a trilingual website with passwordless administration

**Live:** [manalasdungeon.lv](https://manalasdungeon.lv) · **Case study:** [portfolio](https://manalasdungeon.lv/portfolio.php?lang=en)
**Tech:** PHP 8.4 · MySQL · WebAuthn / FIDO2 · OpenSSL · JavaScript · Python (Pillow) · Playwright

A personal site, news and travel blog, Vidzeme travel guide and yoga page — built from scratch without a CMS.

- **Passwordless admin with passkeys (WebAuthn / FIDO2):** the admin pages open only on a registered device with a fingerprint, face or PIN. The server side is plain PHP with no external libraries — CBOR decoding, COSE → PEM key conversion and ES256 / RS256 signature verification with OpenSSL
- **Security following the OWASP Top 10:** PDO prepared statements, output escaping with `htmlspecialchars()`, CSRF tokens on every admin action, session timeouts, HTTPS only, safe image uploads
- **Testing:** 38 unit tests for the passkey cryptography and browser tests with a virtual FIDO2 authenticator (Playwright)
- **Three languages** on every page with hreflang, Open Graph and a multilingual sitemap; clean URLs with mod_rewrite (for example `/linkit`)
- **Private feedback form:** a pop-up `<dialog>` on the home page sends comments straight to email — CSRF token, honeypot, time trap, per-IP and site-wide limits, and email header injection prevention; works without JavaScript too
- **Database-driven content:** news and travel blog in one table with a category, a custom editor with image uploads
- **Image processing with Python (Pillow):** duotone tints, line drawings turned into transparent PNGs, Open Graph images and a QR code

---

### 📚 Manalan Kirjasto — library management system

**Live:** [manalasdungeon.lv/verkkokirjasto](https://manalasdungeon.lv/verkkokirjasto/)
**Tech:** PHP · JavaScript · MySQL · C# WinForms

One library system, built twice: as a web application and as a desktop application sharing one MySQL database.

**Web version**
- Book loans, returns and customer registration, plus an automatic return system run by cron
- Security: SQL injection prevention, PIN hashing with `password_hash()` and `random_int()`, brute-force protection, admin PIN reset and a race-condition fix in customer registration
- PHPUnit test suite with 25 test cases using PDO mocks
- More than 23 defects fixed in code review, including a `GROUP BY` bug in the loan queries
- Gothic dark theme with an animated splash screen; documentation in Word format

**Desktop version (C# WinForms)**
- “Search and lend” workflow
- SSL-protected database connection, typed ListBox objects and an `OperationResult` model for error handling

---

### 🌊 Vitrupes Pludmale — travel website

**Live:** [manalasdungeon.lv/vitrupe](https://manalasdungeon.lv/vitrupe/)
**Tech:** PHP · Bootstrap 5.3 · JavaScript · MySQL · Apache

A travel website about Vitrupe beach on the Vidzeme coast, with a modern design based on traditional Latvian colours and woven-belt patterns.

- **Three languages** (Latvian, English, Finnish) with PHP language files and clean `/en/` and `/fi/` URLs using mod_rewrite
- **Performance:** moving from Bootstrap 4 to 5.3 and removing jQuery cut JavaScript from 252 KB to 80 KB; cache busting with `filemtime`, Apache caching and gzip; optimised photos (32.9 MB → 3.4 MB)
- **SEO:** hreflang, multilingual sitemap, Open Graph and Twitter cards, schema.org `TouristAttraction` structured data
- **Moderated guestbook:** CSRF protection, honeypot, rate limiting, safe link rendering and an admin panel with passkey sign-in where new entries wait for approval
- Image gallery with a lightbox, scroll animations and a sea-sound button

---

### 🐦 Lintujen tunnistus — bird identification game

**Live:** [manalasdungeon.lv/birdgame](https://manalasdungeon.lv/birdgame/)
**Tech:** PHP · JavaScript · CSS

An educational game built for Heinola library’s bus **“Sula”**, where visitors learn to identify Finnish birds.

- 14 bird species, each with its own info card (scientific name, habitat, a fun fact)
- Three languages (Finnish, English, Latvian) with flag buttons for switching
- Questions are shuffled every session; a card interface designed for the library bus

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
- **Portfolio:** [manalasdungeon.lv/portfolio.php](https://manalasdungeon.lv/portfolio.php?lang=en)
- **LinkedIn:** [linkedin.com/in/manalainen](https://www.linkedin.com/in/manalainen/)
- **GitHub:** [github.com/ManalasDungeon](https://github.com/ManalasDungeon)
- **Location:** Heinola, Finland — ready to relocate to Latvia or work remotely
- **Registered in Latvia:** I have a Latvian personal code (personas kods) and an official e-address (e-adrese) on Latvija.gov.lv, which makes hiring and paperwork in Latvia simpler
