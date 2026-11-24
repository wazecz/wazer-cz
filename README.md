# Wazer.cz — One-Page Website Instructions

Edit this file to change content, then ask Claude to regenerate `index.html`.

---

## Design

- **Style:** Modern & clean, Waze brand colors
- **Font:** Rubik (Google Fonts)
- **Colors:**
  - Cyan (primary): `#00CFFF`
  - Navy (dark bg): `#0D1240`
  - Blue (mid): `#1A1F71`
  - Light gray (section bg): `#F4F6F8`
- **Layout:** Single scrollable page, sticky navbar, mobile responsive
- **SEO / head:** canonical `https://www.wazer.cz/`, favicon `/images/waze-icon.svg`, apple-touch-icon `/images/apple-touch-icon.png` (180×180, Waze icon on cyan), theme-color `#0D1240`, Open Graph (og:type, og:url, og:site_name "Wazer.cz", og:title "Wazer.cz — Česká komunita Waze", og:description "Dobrovolná komunita, která tvoří a udržuje mapy Waze v České republice.", og:locale cs_CZ, og:image `/images/og-image.png` 1200×630 — navy, badge "Dobrovolná komunita", "Česká komunita Waze", wazer.cz, Waze icon), twitter:card summary_large_image
- **Robots & sitemap:** `robots.txt` (allow all, points to sitemap) and `sitemap.xml` (index + eu.html) in the root — add new pages to the sitemap
- **Validity:** must pass https://validator.w3.org/nu/ without errors (e.g. no `<div>` inside `<button>` — use `<span>`)
- **Hover:** lift/shadow hover effect only on clickable cards (links, buttons) — never on static cards
- **Meta description:** Dobrovolná komunita, která tvoří a udržuje mapy Waze v České republice a poskytuje českou podporu uživatelům.

---

## Navbar

Links (anchor scroll):
- O nás
- Co děláme
- Zapojit se
- Partneři
- Kontakt

---

## Section 1 — Hero

- **Badge:** Dobrovolná komunita
- **Headline:** Česká komunita Waze
- **Subtext:** Jsme dobrovolníci, kteří tvoří a udržují mapy pro Waze v České republice.
- **Disclaimer (jediná zmínka na webu, lidsky):** Samotnou aplikaci nevyvíjíme — staráme se o to, aby mapa Česka v ní byla co nejpřesnější.
- **Quick action buttons:**
  - 🚧 Hlásit uzavírku → opens modal
  - 🏢 Přidat firmu → opens modal
  - 📱 Stáhnout aplikaci → opens download modal (Google Play / App Store)
  - ✏️ Uprav mapu → anchor scroll to Section 4 (Zapojit se)
- **Action modal content (same structure for Hlásit uzavírku and Přidat firmu):**
  - Modal title (default, replaced by JS): Kontaktujte nás
  - Intro message: "Úprava mapy je jednoduchá. Máme ale spoustu pravidel — pokud si na to netroufáte, dejte nám raději vědět přes jeden z odkazů níže." — "Úprava mapy" is a link that closes the modal and scrolls to Section 4
  - Option 1: Napsat na Facebooku (Přejít do naší Facebook skupiny) → `https://www.facebook.com/groups/629403580825410`
  - Option 2: Napsat na Discordu → `https://discord.gg/cUaGjJY`
  - Option 3: Vyplnit formulář → shows embedded Google Form inline in modal
    - Hlásit uzavírku form: `https://docs.google.com/forms/d/1pRgGg4U97y1PBtByYdBIUf_fiRpayg7goxOdE6NGS9Y/viewform?embedded=true`
    - Přidat firmu form: `https://docs.google.com/forms/d/1YDWLHxvEnNY4tT76KdUHLCs5ZJSs6OOO4lOXpsn8xuQ/viewform?embedded=true`
  - Option 4: Napsat na Waze fóru → `https://www.waze.com/discuss/c/editors/czech-republic-and-slovakia/cz-zadosti-o-upravu-cest-v-cr/4230`
- **Download modal:** Google Play → `https://play.google.com/store/apps/details?id=com.waze` / App Store → `https://apps.apple.com/cz/app/waze-navigation-live-traffic/id323229106`

---

## Section 2 — O nás

- **Label:** O nás
- **Headline:** Kdo jsme?
- **Text paragraph 1:** Jsme **parta lidí z celé republiky** — řidiči, nadšenci do map i úplní začátečníci. Spojuje nás chuť, aby navigace v Česku vedla vždy tou nejlepší cestou.
- **Text paragraph 2:** Mapy ve Waze tvoří dobrovolní editoři po celém světě — lidé, kteří své okolí znají nejlépe. My se staráme o tu českou, od nových obchvatů až po změny jednosměrek. Link on "Waze": `https://www.waze.com`
- **Text paragraph 3:** Udržujeme přímý kontakt s centrálou Waze a pomáháme městům, úřadům i firmám v Česku propojit se s Waze — třeba při sdílení uzavírek a dopravních dat.
- **Stat cards:**
  - 800+ tis. / editací mapy v ČR ročně
  - 20 / aktivních členů komunity
  - 6 / partnerských organizací
  - 100% / dobrovolníci

---

## Section 3 — Co děláme

- **Label:** Naše aktivity
- **Headline:** Co děláme
- **Cards (4):**
  1. **Tvorba map** — Editujeme a udržujeme silniční síť České republiky — nové silnice, opravy chyb, rychlostní limity.
  2. **Hlášení uzavírek** — Zpracováváme hlášení o uzavírkách od řidičů i partnerů a promítáme je do map v reálném čase.
  3. **Podpora uživatelů** — Odpovídáme na dotazy v česko-slovenském fóru a pomáháme řidičům s Waze v češtině.
  4. **Překlady** — Překládáme rozhraní Waze a wiki dokumentaci do češtiny, aby bylo vše dostupné v mateřském jazyce.

---

## Section 4 — Zapojit se

- **Label:** Komunita
- **Headline:** Zapojit se
- **Subtext:** Chcete přispět k lepší navigaci v Česku? Tady je jak.
- **Action cards (3):**
  1. **Editor map** — Opravujte silnice, přidávejte nové ulice a vylepšujte mapy přímo ve Waze Map Editoru. → `https://www.waze.com/cs/editor`
  2. **Školení editorů** — Naučte se základy editace map v češtině — od silnic po místa zájmů. → `https://wazeopedia.waze.com/wiki/Czech/Školení`
  3. **CS/SK Fórum** — Diskutujte s ostatními editory, ptejte se a sdílejte tipy v česko-slovenské komunitě. → `https://www.waze.com/discuss/c/editors/czech-republic-and-slovakia/4229`
- **Donation banner:**
  - Headline: Podpořte nás
  - Text: Naše komunita funguje čistě dobrovolnicky. Pokud chcete podpořit provoz webu a aktivity, budeme rádi za každou korunu. Příspěvky přijímáme na transparentní účet spolku u Fio banky.
  - Button: ❤️ Přispět → `https://ib.fio.cz/ib/transparent?a=2603601701`

---

## Section 5 — Partneři

- **Label:** Spolupráce
- **Headline:** Partneři
- **Subtext:** Spolupracujeme s organizacemi, které sdílejí dopravní data a zlepšují Waze pro české řidiče.
- **Partners (6) — each card has logo + name + description** (cards are not links → no hover effect)
  - Logo files are in `logos/` folder (SVG with explicit width/height attributes — without them the logo collapses to 0), displayed 48px high / max 160px wide, left-aligned
  - Logo and name link to the partner website (new tab); the card itself is not a link

| # | Name | Link | Logo file | Description |
|---|------|------|-----------|-------------|
| 1 | ŘSD | `https://rsd.cz` | `logos/rsd.svg` | Ředitelství silnic a dálnic sdílí přes Jednotný systém dopravních informací (JSDI) data o uzavírkách a omezeních na dálnicích a silnicích I. třídy. |
| 2 | Město Brno | `https://www.brno.cz` | `logos/brno.svg` | První česká obec v programu Waze for Cities — sdílí s námi data o uzavírkách a dopravních omezeních ve městě. |
| 3 | ČÚZK | `https://cuzk.gov.cz` | `logos/cuzk.svg` | Český úřad zeměměřický a katastrální poskytuje kartografické podklady, ze kterých vycházíme při tvorbě a aktualizaci map. |
| 4 | RunCzech | `https://www.runczech.com` | `logos/runczech.svg` | Pořadatel běžeckých závodů. Uzavírky tratí promítáme do Waze předem, aby je řidiči mohli včas objet. |
| 5 | Rally – Mediasport | — (chybí) | `logos/mediasport.svg` (chybí — zatím textový placeholder) | Pořadatel rally závodů sdílí uzavírky rychlostních zkoušek, aby se jim řidiči mohli s Waze včas vyhnout. |
| 6 | Waze Slovensko | `https://www.facebook.com/waze.sk` | `images/waze-icon.svg` | Slovenská sesterská komunita — sdílíme fórum, pravidla editace i zkušenosti. |

- **Last tile — CTA (navy, full-width banner under the partner cards):**
  - Headline: Staňte se partnerem
  - Text: Pořádáte akci, spravujete silnice nebo máte dopravní data? Ozvěte se nám — pomůžeme dostat aktuální uzavírky a dopravní informace do Waze.
  - Button: Napsat na info@wazer.cz → `mailto:info@wazer.cz?subject=Spolupráce s Waze ČR`

---

## Section 6 — Kontakt

- **Label:** Kontakt
- **Headline:** Kontakt
- **Layout:** 2-column grid

### Left column
- **"Informace o spolku" button** — opens modal (see below)
- **Email:** info@wazer.cz → `mailto:info@wazer.cz`

### Right column — Social links
| Platform | URL |
|----------|-----|
| Facebook — stránka | `https://www.facebook.com/WazeCZ` |
| Facebook — skupina | `https://www.facebook.com/groups/629403580825410` |
| Discord | `https://discord.gg/cUaGjJY` |

### "Informace o spolku" modal
**Výbor (5 members)** — displayed as nickname (bold) + real name (small gray below)

| Initial | Nickname | Real name |
|---------|----------|-----------|
| P | GinBook | Patrik Ingr |
| V | vitj | Vít Jelínek |
| M | MajkiiTelini | Michal Telenský |
| M | masvbr | Martin Svoboda |
| M | martinkolar | Martin Kolář |

**Informace o spolku**
Údaje dle ARES (https://ares.gov.cz/ekonomicke-subjekty?ico=29688876):
- **Název:** Spolek editorů Waze Česká republika, z.s.
- **IČO:** 29688876
- **Transparentní účet:** 2603601701 / 2010 (Fio banka, majitel: spolek) — číslo je odkaz → `https://ib.fio.cz/ib/transparent?a=2603601701`
- **Sídlo:** Uralská 689/7, Bubeneč, 160 00 Praha 6
- **Zápis ve spolkovém rejstříku:** L 82200 vedená u Městského soudu v Praze

**Donate section** (inside modal, navy card)
- Headline: ❤️ Podpořte nás
- Text: Naše komunita funguje čistě dobrovolnicky. Přijmeme každou korunu — na transparentní účet spolku u Fio banky.
- Button: Přispět → `https://ib.fio.cz/ib/transparent?a=2603601701`

---

## Footer

- **Text:** © [auto year] Wazer.cz — dobrovolná komunita Waze ČR
- **Left links (right after the text, new tab):**
  - Sbírka listin → `https://or.justice.cz/ias/ui/vypis-sl-firma?subjektId=1324341`
  - Stanovy spolku → `https://or.justice.cz/ias/ui/vypis-sl-detail?dokument=91891542&subjektId=1324341&spis=1496121`
- **Right links:**
  - Komunity v Evropě → `eu.html`
  - Waze.com → `https://www.waze.com`

---

## Subpage — eu.html (European Waze Communities)

Remake of the old `https://wazer.cz/eu/` page in the same design as `index.html`. English (international audience).

- **Title:** European Waze Communities — Wazer.cz
- **Head:** canonical `https://www.wazer.cz/eu.html`, same favicon / apple-touch-icon / theme-color / og:image as index, Open Graph (title "Waze Europe" + description, og:locale en_GB), twitter:card summary_large_image
- **Navbar:** Wazer.cz logo → `index.html`, link "← Česká komunita" → `index.html`
- **Hero:** badge "Waze Europe", headline "European Waze Communities", subtext "Find the volunteer Waze community in your country — websites, social media, wiki and forums."
- **Search box:** "Search country…" — filters cards by English or local name; empty state "No country found."
- **Country cards:** flag (flagcdn.com), English name (links to the community website if any), local name in italics, link pills: Website, Facebook, X, Chat, Stats, Wiki, Forum, YouTube. Countries without links are dimmed with "No community links yet".
- **Data:** `countries` array in the `<script>` of `eu.html` — edit there to add/change countries or links. Google+ links from the old page were removed (service shut down). Czechia links to `index.html` and uses current Discord + Discuss forum.
- **Footer:** Waze Map Editor → `https://www.waze.com/editor` · Community Forums → `https://www.waze.com/discuss/` · © [auto year] Waze ČR → `index.html` · "Maintained by users — not an official Waze site."
