# TODO — Wazer.cz

## Odkazy
- [ ] **Wazeopedia** — odkazy `wazeopedia.waze.com/wiki/...` (index.html: Školení editorů; eu.html: Wiki u všech zemí) jen přesměrovávají přes legacy redirector Waze (při kontrole vracely 429). Najít aktuální adresy a nahradit.
- [ ] **Staré fórum** — v eu.html mají ostatní země odkazy `waze.com/forum/viewforum.php?f=...`, které také jen přesměrovávají. Nahradit adresami `waze.com/discuss/...`.
- [ ] **Mrtvé/neověřené odkazy v eu.html** — Slack workspace (Belarus, Benelux), `wazerussia.tk`, `hamsterpad.com` (Latvia), statistiky (wazebelgium.be/stat, statystyki.mouse.one.pl, stats.waze.su), weby národních komunit. Projít a nefunkční odstranit.

## Obsah
- [ ] **Litva v eu.html** — odkazuje na lotyšský Facebook (`WazeLv`) a má stejné fórum jako Estonsko (`f=1347`). Chyba převzatá z původní stránky — doplnit správné odkazy.
- [ ] **Logo Waze Slovensko** — wazer.sk vrací „Access Forbidden“, zatím je použitá ikona Waze (`images/waze-icon.svg`). Případně dodat logo SK komunity.
- [ ] **Rally – Mediasport** — dodat web (odkaz na logu a názvu), logo (`logos/mediasport.svg`, pak odkomentovat `<img>` v index.html) a ověřit text karty.
- [ ] **Texty partnerů** — ověřit formulace (Brno ve Waze for Cities, ŘSD přes JSDI, RunCzech).

## Server (nginx)
- [ ] **Neexistující URL vrací 302 na homepage** — např. `/neexistuje`, `/robots.txt`, `/favicon.ico`. Google to bere jako „soft 404“. Nastavit, aby neexistující stránky vracely **404** (ideálně s vlastní 404 stránkou).
- [ ] **Staré `/eu/` → `/eu.html`** — teď `/eu/` přesměrovává 302 na homepage. Nastavit **301** na `https://www.wazer.cz/eu.html` (staré odkazy z jiných komunit).
- [ ] **Po nasazení ověřit** `https://www.wazer.cz/robots.txt` a `/sitemap.xml` — musí vracet 200, ne přesměrování. Pak sitemap přidat do Google Search Console.
- [ ] **Bezpečnostní hlavičky** — přidat do nginx:
  ```nginx
  add_header Strict-Transport-Security "max-age=31536000" always;
  add_header X-Content-Type-Options "nosniff" always;
  add_header Referrer-Policy "strict-origin-when-cross-origin" always;
  add_header X-Frame-Options "SAMEORIGIN" always;
  ```
- [ ] **Charset v Content-Type** — server posílá `Content-Type: text/html` bez kódování. Přidat `charset utf-8;` (stránky mají `<meta charset>`, takže to funguje, ale je to čistší).
- [ ] **HTTP/2** — server odpovídá jen HTTP/1.1. Zapnout `http2 on;` (rychlejší načítání více souborů najednou).
- [ ] **Cache pro obrázky** — `logos/`, `images/` posílat s `Cache-Control: public, max-age=2592000` (teď jen ETag).
- [ ] **https://wazer.cz → www** používá 301, ale http:// varianty 308 — funguje, jen pro pořádek sjednotit na 301.

## Technické
- [ ] **Tailwind přes CDN** — `cdn.tailwindcss.com` není určený pro produkci. Zvážit build přes Tailwind CLI (vygenerovaný CSS soubor).
