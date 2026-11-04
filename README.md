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
- **Subtext:** Jsme dobrovolníci, kteří tvoří a udržují mapy pro Waze v České republice a poskytují českou podporu uživatelům.
- **Disclaimer:** Nejsme tvůrci aplikace Waze — ta patří společnosti Waze Mobile (Google).
- **Quick action buttons:**
  - 🚧 Hlásit uzavírku → opens modal
  - 🏢 Přidat firmu → opens modal
  - 📱 Stáhnout aplikaci → opens download modal (Google Play / App Store)
  - ✏️ Uprav mapu → anchor scroll to Section 4 (Zapojit se)
- **Action modal content (same structure for Hlásit uzavírku and Přidat firmu):**
  - Intro message: "Úprava mapy je jednoduchá. Máme ale spoustu pravidel — pokud se na to necítíš, dej nám raději vědět na jednom z odkazů níže." — "Úprava mapy" is a link that closes the modal and scrolls to Section 4
  - Option 1: Napsat na Facebooku → `https://www.facebook.com/groups/629403580825410`
  - Option 2: Napsat na Discordu → `https://discord.gg/cUaGjJY`
  - Option 3: Vyplnit formulář → shows embedded Google Form inline in modal
    - Hlásit uzavírku form: `https://docs.google.com/forms/d/1pRgGg4U97y1PBtByYdBIUf_fiRpayg7goxOdE6NGS9Y/viewform?embedded=true`
    - Přidat firmu form: `https://docs.google.com/forms/d/1YDWLHxvEnNY4tT76KdUHLCs5ZJSs6OOO4lOXpsn8xuQ/viewform?embedded=true`
  - Option 4: Napsat na Waze fóru → `https://www.waze.com/discuss/c/editors/czech-republic-and-slovakia/cz-zadosti-o-upravu-cest-v-cr/4230`
- **Download modal:** Google Play → `https://play.google.com/store/apps/details?id=com.waze` / App Store → `https://itunes.apple.com/cz/app/waze-social-gps-traffic/id323229106`

---

## Section 2 — O nás

- **Label:** O nás
- **Headline:** Kdo jsme?
- **Text paragraph 1:** Jsme dobrovolná komunita nadšenců, kteří se starají o mapy Waze v České republice. Opravujeme silnice, doplňujeme nové ulice, hlásíme uzavírky a překládáme Waze do češtiny.
- **Text paragraph 2:** Waze je navigační aplikace od společnosti Waze Mobile (vlastněné Googlem od roku 2013). My tuto aplikaci nevyvíjíme — jsme nezávislá komunita, která ji vylepšuje zevnitř jako editori map a koordinátoři. Link: `https://www.waze.com`
- **Text paragraph 3:** Udržujeme přímý kontakt s centrálou Waze v Izraeli a koordinujeme aktivity s česky mluvícími kolegy ze Slovenska.
- **Stat cards:**
  - 800+ tis. / editací mapy v ČR ročně
  - 20 / aktivních LC členů
  - 9+ / Partnerských organizací
  - 100% / Dobrovolníci

---

## Section 3 — Co děláme

- **Label:** Naše aktivity
- **Headline:** Co děláme
- **Cards (4):**
  1. **Tvorba map** — Editujeme a udržujeme silniční síť České republiky — nové silnice, opravy chyb, rychlostní limity.
  2. **Hlášení uzavírek** — Zpracováváme hlášení o uzavírkách od řidičů i partnerů a promítáme je do map v reálném čase.
  3. **Podpora uživatelů** — Odpovídáme na dotazy v česko-slovenském fóru a pomáháme řidičům s Waze v jejich jazyce.
  4. **Překlady** — Překládáme rozhraní Waze a wiki dokumentaci do češtiny, aby bylo vše dostupné v mateřském jazyce.

---

## Section 4 — Zapojit se

- **Label:** Komunita
- **Headline:** Zapojit se
- **Subtext:** Chcete přispět k lepší navigaci v Česku? Tady je jak.
- **Action cards (3):**
  1. **Editor map** — Opravujte silnice, přidávejte nové ulice a vylepšujte mapy přímo ve Waze Map Editoru. → `https://www.waze.com/cs/editor`
  2. **Školení editorů** — Naučte se základy editace map v češtině — od silnic po místa zájmů. → `https://wazeopedia.waze.com/wiki/Czech/Školení`
  3. **CS/SK Fórum** — Diskutujte s ostatními editory, ptejte se a sdílejte tipy v česko-slovenské komunitě. → `https://www.waze.com/forum/viewforum.php?f=22`
- **Donation banner:**
  - Headline: Podpořte nás
  - Text: Naše komunita funguje čistě dobrovolnicky. Pokud chcete podpořit provoz webu a aktivity, přijmeme každou korunou. Transparentní účet Fio banky.
  - Button: ❤️ Přispět → `https://ib.fio.cz/ib/transparent?a=2900907010`

---

## Section 5 — Partneři

- **Label:** Spolupráce
- **Headline:** Partneři
- **Subtext:** Spolupracujeme s organizacemi, které sdílejí dopravní data a zlepšují Waze pro české řidiče.
- **Partners (9) — each card has a logo slot + name + description:**
  - Logo file goes in `logos/` folder, referenced as `<img src="logos/filename.png">`
  - Format: `logos/<slug>.png`, max display height 40px

| # | Name | Logo file | Description |
|---|------|-----------|-------------|
| 1 | Radio Impuls | `logos/radio-impuls.png` | Integruje hlášení Waze do dopravní rubriky „Doprava 007". |
| 2 | Město Brno | `logos/brno.png` | První česká obec v programu Connected Citizens — sdílí data o uzavírkách. |
| 3 | RunCzech | `logos/runczech.png` | Sdílí data o uzavírkách při běžeckých závodech, aby řidiči mohli objíždět trasy. |
| 4 | JSDI | `logos/jsdi.png` | Výměna dat o dopravních uzavírkách přes jednotný dopravní informační systém. |
| 5 | ŘSD | `logos/rsd.png` | Ředitelství silnic a dálnic poskytuje mapová data a podporuje Waze Beacons. |
| 6 | ČÚZK | `logos/cuzk.png` | Poskytuje kartografické podklady pro tvorbu a aktualizaci map. |
| 7 | Pretol | `logos/pretol.png` | Odtahová služba sdílí aktuální informace o nehodách a zácpách na dálnicích. |
| 8 | Petra Biache | `logos/petra-biache.png` | Hlasová profesionálka — hlas české verze klasické navigace Waze. |
| 9 | Waze Slovensko | `logos/waze-sk.png` | Slovenská sesterská komunita — pravidelná spolupráce a sdílení zkušeností. |

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
- **Název:** Název spolku, z.s.
- **IČO:** 00000000
- **Sídlo:** Ulice 1, 000 00 Město
- **Bankovní účet:** 0000000000 / 0000

**Donate section** (inside modal, navy card)
- Headline: ❤️ Podpořte nás
- Text: Naše komunita funguje čistě dobrovolnicky. Přijmeme každou korunu — transparentní účet Fio banky.
- Button: Přispět → `https://ib.fio.cz/ib/transparent?a=2900907010`

---

## Footer

- **Text:** © [auto year] Wazer.cz — dobrovolná komunita Waze ČR
- **Disclaimer:** Nejsme Waze ani Google.
- **Link:** Waze.com → `http://www.waze.com`
