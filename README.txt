Návod: nasazení na GitHub Pages (zdarma)
=========================================

Co v balíčku je:
- index.html   -> samotná aplikace
- manifest.json -> aby šla "Přidat na plochu" jako appka
- sw.js        -> offline cache (funguje i bez signálu v posilovně)
- icon-192.png, icon-512.png -> ikony appky

KROKY (bez příkazové řádky, jen přes web GitHubu):

1. Jdi na https://github.com a založ si účet, pokud ho nemáš.

2. Klikni vpravo nahoře na "+" -> "New repository".
   - Repository name: např. ppl-plan
   - Public
   - NEZAŠKRTÁVEJ "Add a README file"
   - Klikni "Create repository"

3. Na stránce nového (prázdného) repozitáře uvidíš odkaz
   "uploading an existing file" - klikni na něj.
   (Nebo: Add file -> Upload files)

4. Přetáhni tam všech 5 souborů z tohoto balíčku najednou
   (index.html, manifest.json, sw.js, icon-192.png, icon-512.png).
   Dole klikni "Commit changes".

5. Jdi do Settings (nahoře v repozitáři) -> vlevo dole "Pages".
   - Branch: main
   - Folder: / (root)
   - Klikni Save.

6. Počkej cca 1-2 minuty a obnov stránku Settings -> Pages.
   Objeví se tam zelený odkaz typu:
   https://TVOJE-JMENO.github.io/ppl-plan/

7. Otevři ten odkaz na mobilu i na PC.
   Na mobilu (Chrome/Safari) použij "Přidat na plochu" / "Add to Home Screen"
   - appka pak bude fungovat jako normální ikona, i offline.

DŮLEŽITÉ - žádná automatická synchronizace mezi zařízeními:
Mobil a PC mají každý svoje vlastní uložiště v prohlížeči (localStorage).
Když si zapíšeš váhu na mobilu, na PC se needo automaticky. Použij tlačítka
Export / Import v appce, abys přenesl zálohu z jednoho zařízení na druhé.

Pokud budeš chtít v budoucnu upravit plán (přidat/změnit cvik), stačí mi dát
vědět, upravím index.html a pošlu ti nový, ty ho jen znovu nahraješ do
stejného GitHub repozitáře (přepíše starý soubor, appka se sama aktualizuje).
