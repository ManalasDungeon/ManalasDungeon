[🇬🇧 English](README.md) · **🇱🇻 Latviešu**

# Marko Nakari (Mana)

**Programmatūras izstrādātājs** · Heinola, Somija · Meklēju darbu Latvijā (Vidzemē vai attālināti)

[🌐 manalasdungeon.lv](https://manalasdungeon.lv) · [✉️ marko.nakari@inbox.lv](mailto:marko.nakari@inbox.lv) · [💼 LinkedIn](https://www.linkedin.com/in/manalainen/) · [🐙 GitHub](https://github.com/ManalasDungeon)

---

## Par mani

Programmatūras izstrādātājs, 2026. gada 1. oktobrī absolvēju **Vamia**. Kopš 2006. gada strādāju Heinolas bibliotēkā Somijā, bet kopš 2025. gada aprīļa — par mediju instruktoru. Līdztekus darbam bibliotēkā esmu izstrādājis programmatūru, ko izmanto bibliotēkas apmeklētāji.

Mana stiprākā joma ir **PHP/MySQL tīmekļa izstrāde LAMP vidē un koplietošanas hostingā** (cPanel, phpMyAdmin, Apache konfigurācija). Veidoju arī darbvirsmas lietotnes ar C#/.NET. Man rūp drošs kods, testēšana un ātras, labi indeksētas tīmekļa vietnes.

## Darba pieredze

| | |
|---|---|
| **Mediju instruktors (Mediaohjaaja)** | Heinolas bibliotēka · 04/2025 – šobrīd |
| **Bibliotēkas darbinieks (Kirjastovirkailija)** | Heinolas bibliotēka · 2006 – 2025 |

## Izglītība

| | |
|---|---|
| **Programmatūras izstrādātājs (Ohjelmistokehittäjä)** | Vamia, attālinātās studijas · 2026 |
| **Bibliotēkas merkonoms (Kirjastomerkonomi)** | Profesionālā izglītība · 1996 |
| **Vidējā izglītība (Ylioppilas)** | Somijas vidusskolas gala eksāmeni · 1991 |

## Tehnoloģijas

| Joma | Tehnoloģijas |
|---|---|
| Programmēšanas valodas | PHP, JavaScript, C#, Kotlin, Python, SQL |
| Tīmeklis | HTML5, CSS3, Bootstrap 5, vanilla JS |
| Serveris | Apache (mod_rewrite, .htaccess, kešošana, gzip), cron, cPanel |
| Datubāzes | MySQL, PDO, phpMyAdmin, MySQL Connector/NET |
| Darbvirsma | .NET WinForms |
| Testēšana | PHPUnit |
| SEO | Open Graph, schema.org JSON-LD, hreflang, vietnes kartes (sitemap) |

---

## Galvenie projekti

### 📚 Manalan Kirjasto — bibliotēkas pārvaldības sistēma

**Tiešsaistē:** [manalasdungeon.lv/verkkokirjasto](https://manalasdungeon.lv/verkkokirjasto/)
**Tehnoloģijas:** PHP · JavaScript · MySQL · C# WinForms

Viena bibliotēkas sistēma, izveidota divreiz: kā tīmekļa lietotne un kā darbvirsmas lietotne ar kopīgu MySQL datubāzi.

**Tīmekļa versija**
- Grāmatu izsniegšana, atgriešana un klientu reģistrācija, kā arī automātiska atgriešanas sistēma, ko darbina cron
- Drošība: SQL injekciju novēršana, PIN kodu jaukšana ar `password_hash()` un `random_int()`, aizsardzība pret brute-force uzbrukumiem, administratora PIN atiestatīšana un sacensību stāvokļa (race condition) labojums klientu reģistrācijā
- PHPUnit testu komplekts ar 25 testgadījumiem, izmantojot PDO imitācijas (mocks)
- Koda pārskatīšanā izlaboti vairāk nekā 23 trūkumi, tostarp `GROUP BY` kļūda izsniegumu vaicājumos
- Gotiska tumšā tēma ar animētu sākuma ekrānu; dokumentācija Word formātā

**Darbvirsmas versija (C# WinForms)**
- Darba plūsma "meklēt un izsniegt"
- Ar SSL aizsargāts datubāzes savienojums, tipizēti ListBox objekti un `OperationResult` modelis kļūdu apstrādei

---

### 🌊 Vitrupes Pludmale — tūrisma vietne

**Tiešsaistē:** [manalasdungeon.lv/vitrupe](https://manalasdungeon.lv/vitrupe/)
**Tehnoloģijas:** PHP · Bootstrap 5.3 · JavaScript · MySQL · Apache

Tūrisma vietne par Vitrupes pludmali Vidzemes piekrastē ar modernu dizainu, kura pamatā ir tradicionālās latviešu krāsas un prievīšu raksti.

- **Trīs valodas** (latviešu, angļu, somu) ar PHP valodu failiem un tīriem `/en/` un `/fi/` URL, izmantojot mod_rewrite
- **Veiktspēja:** pāreja no Bootstrap 4 uz 5.3 un jQuery noņemšana samazināja JavaScript apjomu no 252 KB līdz 80 KB; kešatmiņas atjaunošana ar `filemtime`, Apache kešošana un gzip; optimizēti foto (32,9 MB → 3,4 MB)
- **SEO:** hreflang, daudzvalodu vietnes karte, Open Graph un Twitter kartītes, schema.org `TouristAttraction` strukturētie dati
- **Viesu grāmata ar moderāciju:** CSRF aizsardzība, honeypot, pieprasījumu skaita ierobežošana, droša saišu attēlošana un ar bcrypt aizsargāts administratora panelis, kur jauni ieraksti gaida apstiprinājumu
- Attēlu galerija ar lightbox, ritināšanas animācijas un jūras skaņu poga

---

### 🐦 Lintujen tunnistus — putnu atpazīšanas spēle

**Tiešsaistē:** [manalasdungeon.lv/birdgame](https://www.manalasdungeon.lv/birdgame/)
**Tehnoloģijas:** PHP · JavaScript · CSS

Izglītojoša spēle, kas izveidota Heinolas bibliotēkas autobusam **"Sula"**, kur apmeklētāji mācās atpazīt Somijas putnus.

- 14 putnu sugas, katrai sava informācijas kartīte (zinātniskais nosaukums, dzīvotne, interesants fakts)
- Trīs valodas (somu, angļu, latviešu) ar karogu pogām valodas pārslēgšanai
- Jautājumi katrā sesijā tiek sajaukti; kartīšu saskarne, kas pielāgota bibliotēkas autobusam

---

## Valodas

| Valoda | Līmenis |
|---|---|
| Somu | Dzimtā valoda |
| Angļu | Brīvi |
| Latviešu | Pamatzināšanas |
| Zviedru | Pamatzināšanas |

## Kontakti

- **E-pasts:** marko.nakari@inbox.lv
- **Tīmekļa vietne:** [manalasdungeon.lv](https://manalasdungeon.lv)
- **LinkedIn:** [linkedin.com/in/manalainen](https://www.linkedin.com/in/manalainen/)
- **GitHub:** [github.com/ManalasDungeon](https://github.com/ManalasDungeon)
- **Atrašanās vieta:** Heinola, Somija — gatavs pārcelties uz Latviju vai strādāt attālināti
