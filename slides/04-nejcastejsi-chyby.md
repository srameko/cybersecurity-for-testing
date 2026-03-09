---
layout: section
---
# Nejčastější chyby
## Které můžete potkat

---
layout: default
---
# Slabá nebo výchozí hesla

| | |
|---|---|
| **Problém** | Uživatelský účet „chráněný" jednoduchým heslem (123456, admin/admin) |
| **Dopad** | Útočník se snadno přihlásí → získá přístup k účtu |
| **Příklad** | Zadáním „slabého" hesla se může přihlásit kdokoli |
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
| **Vyzkoušej** | [TOTP Challenge](https://authenticationtest.com/totpChallenge/) |

---
layout: default
---
# Jak nemá MFA vypadat

<img src="/mfa.png" class="mx-auto" style="max-height: 80%; width: 80%; object-fit: contain;" />
---
layout: default
---
# Nešifrovaná komunikace (HTTP)

| | |
|---|---|
| **Problém** | Data cestují mezi uživatelem a serverem nezabezpečeně |
| **Dopad** | Útočník může odposlechnout hesla a citlivá data (PII) |
| **Příklad** | Přihlášení k účtu přes veřejnou Wi-Fi |
| **Jak ověřit** | Podívat se, zda web běží na `https://` a má důvěryhodný certifikát |
| **Vyzkoušej** | [badssl.com](https://badssl.com/) |

---
layout: default
---
# SQL Injection (SQLi)

| | |
|---|---|
| **Problém** | Zadání vstupu přímo do databázového dotazu |
| **Dopad** | Útočník může číst, měnit nebo mazat data v databázi |
| **Příklad** | `' OR '1'='1` v přihlašovacím formuláři |
| **Jak ověřit** | Do pole vložit `' OR '1'='1` a sledovat co se stane |
| **Demo** | [Hacksplaining - SQLi](https://www.hacksplaining.com/lessons/sql-injection/start) |

---
layout: default
---
# Cross-Site Scripting (XSS)

| | |
|---|---|
| **Problém** | Útočník vloží JavaScript do stránky |
| **Dopad** | Může krást přihlášení nebo manipulovat obsahem |
| **Příklad** | Komentář `<script>alert(1)</script>` |
| **Jak ověřit** | Otestovat vložením skriptu do textového pole |
| **Demo** | [Hacksplaining - XSS](https://www.hacksplaining.com/lessons/xss-stored/start) |

---
layout: default
---
# Cross-Site Request Forgery (CSRF)

| | |
|---|---|
| **Problém** | Útočník přiměje uživatele k akci bez jeho vědomí |
| **Dopad** | Nechtěná akce jménem uživatele (např. převod peněz) |
| **Příklad** | Skrytý odkaz v e-mailu změní nastavení účtu |
| **Jak ověřit** | Podívat se, zda má formulář unikátní CSRF token |
| **Demo** | [Hacksplaining - CSRF](https://www.hacksplaining.com/lessons/csrf/start) |

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
# Přidejte si admina (Driver categorization FIA)

<div class="grid grid-cols-2 gap-4 mt-4">
  <img src="/sqli-fia-1.png" style="object-fit: contain; max-height: 75%; width: 80%;" />
  <img src="/sqli-fia-2.png" style="object-fit: contain; max-height: 75%; width: 80%;" />
</div>
---
layout: default
---
# Nahrávání nebezpečných souborů

| | |
|---|---|
| **Problém** | Server povolí nahrát libovolný soubor |
| **Dopad** | Útočník spustí vlastní kód a ovládne server |
| **Příklad** | Nahrání web shellu |
| **Jak ověřit** | Zkusit nahrát neobvyklý soubor (např. EXE, EICAR, …) |

---
layout: default
---
# Zastaralé knihovny

| | |
|---|---|
| **Problém** | Používání starých verzí softwaru |
| **Dopad** | Útočník využije známé chyby a pronikne do systému |
| **Příklad** | Stará verze jQuery s veřejnou zranitelností |
| **Jak ověřit** | Podívat se na verze knihoven (např. zdrojový kód webu) |
| **Zdroje** | [CVE Details](https://www.cvedetails.com/) · [National Vulnerability Database](https://nvd.nist.gov/vuln/) · [Snyk Security Database](https://security.snyk.io/) |

---
layout: default
---
# Nesprávně nastavený server

| | |
|---|---|
| **Co to je** | Server odhaluje příliš mnoho informací nebo je špatně nastavený |
| **Co způsobí** | Útočník získá detaily, které mu pomohou s útokem |
| **Příklad** | Chybová hláška ukáže SQL dotaz, heslo nebo konfiguraci |
| **Jak ověřit** | Využijte funkci zapomenuté heslo — přijde vám heslo čitelné? |
| **Zdroje** | [Jak jsou uložena hesla](https://pulse.michalspacek.cz/passwords/storages) |
---
layout: default
---
# Příklad výpisu chyby

<img src="/error.png" class="mx-auto mt-2" style="max-height: 80%; width: 80%; object-fit: contain;" />
---
layout: image
image: /kahoot-pentest.png
---
