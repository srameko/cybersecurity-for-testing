---
layout: section
subtitle: Které můžete potkat
---
# Nejčastější chyby
---
layout: default
---
# Slabá nebo výchozí hesla

| | |
|---|---|
| **Problém** | Účet „chráněný" heslem 123456 nebo admin/admin |
| **Dopad** | Útočník se snadno přihlásí |
| **Příklad** | Zadáním slabého hesla se může přihlásit kdokoli |
| **Jak ověřit** | Zkusit nastavit nebo použít jednoduché heslo |
---
layout: default
---
# Chybějící vícefaktorové ověření (MFA)

| | |
|---|---|
| **Problém** | Přístup chráněný jen heslem |
| **Dopad** | Pokud unikne heslo → útočník se dostane do systému |
| **Příklad** | Ukradené heslo ze špatně zabezpečeného webu / infostealer |
| **Jak ověřit** | Zkontrolovat, zda aplikace podporuje MFA (OTP / Passkeys) |
---
layout: default
---
# Nešifrovaná komunikace (HTTP)

| | |
|---|---|
| **Problém** | Data cestují nezabezpečeně |
| **Dopad** | Útočník může odposlechnout hesla a citlivá data (PII) |
| **Příklad** | Přihlášení k účtu přes veřejnou Wi-Fi |
| **Jak ověřit** | Podívat se, zda web běží na `https://` a má důvěryhodný certifikát |
---
layout: default
---
# SQL Injection (SQLi)

| | |
|---|---|
| **Problém** | Zadání vstupu přímo do databázového dotazu |
| **Dopad** | Útočník může číst, měnit nebo mazat data v databázi |
| **Příklad** | `' OR '1'='1` v přihlašovacím formuláři |
| **Jak ověřit** | Vložit `' OR '1'='1` a sledovat co se stane |
| **Demo** | Hacksplaining - SQLi |
---
layout: default
---
# Cross-Site Scripting (XSS)

| | |
|---|---|
| **Problém** | Útočník vloží JavaScript do stránky |
| **Dopad** | Může krást přihlášení nebo manipulovat obsahem |
| **Příklad** | `<script>alert(1)</script>` v komentáři |
| **Jak ověřit** | Otestovat vložením skriptu do textového pole |
| **Demo** | Hacksplaining - XSS |
---
layout: default
---
# Cross-Site Request Forgery (CSRF)

| | |
|---|---|
| **Problém** | Útočník přiměje uživatele k akci bez jeho vědomí |
| **Dopad** | Nechtěná akce jménem uživatele (např. převod peněz) |
| **Příklad** | Skrytý odkaz v e-mailu změní nastavení účtu |
| **Jak ověřit** | Zkontrolovat, zda má formulář unikátní CSRF token |
| **Demo** | Hacksplaining - CSRF |
---
layout: default
---
# Špatná správa oprávnění

| | |
|---|---|
| **Problém** | Uživatel se dostane k funkcím, které nemá mít |
| **Dopad** | Běžný uživatel získá přístup k datům admina |
| **Příklad** | Otevření URL `/admin` bez administrátorských oprávnění |
| **Jak ověřit** | Přihlásit se jako běžný uživatel a zkusit admin URL |
---
layout: default
---
# Nahrávání nebezpečných souborů

| | |
|---|---|
| **Problém** | Server povolí nahrát libovolný soubor |
| **Dopad** | Útočník spustí vlastní kód a ovládne server |
| **Příklad** | Nahrání web shellu |
| **Jak ověřit** | Zkusit nahrát neobvyklý soubor (EXE, EICAR, …) |
---
layout: default
---
# Zastaralé knihovny

| | |
|---|---|
| **Problém** | Používání starých verzí softwaru |
| **Dopad** | Útočník využije známé chyby |
| **Příklad** | Stará verze jQuery s veřejnou zranitelností |
| **Jak ověřit** | Podívat se na verze knihoven ve zdrojovém kódu webu |

**Zdroje:** CVE Details · National Vulnerability Database · Snyk Security Database
---
layout: default
---
# Nesprávně nastavený server

| | |
|---|---|
| **Problém** | Server odhaluje příliš mnoho informací |
| **Dopad** | Útočník získá detaily, které mu pomohou s útokem |
| **Příklad** | Chybová hláška ukáže SQL dotaz, heslo nebo konfiguraci |
| **Jak ověřit** | Využijte funkci zapomenuté heslo — přijde vám heslo čitelné? |
