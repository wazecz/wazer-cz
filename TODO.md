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

## Technické
- [ ] **Tailwind přes CDN** — `cdn.tailwindcss.com` není určený pro produkci. Zvážit build přes Tailwind CLI (vygenerovaný CSS soubor).
