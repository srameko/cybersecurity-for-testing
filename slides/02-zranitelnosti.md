---
layout: section
---
# Zranitelnosti
---
layout: default
---
# Životní cyklus zranitelnosti

<v-clicks>

1. **Objev** — najdete zranitelnost
2. **Report výrobci** (Bug bounty)
3. **Potvrzení + odměna**
4. **Oprava za 30–90 dní** (update / patch)

</v-clicks>
---
layout: default
---
# Označení zranitelnosti — CVE

Po ověření je přiřazeno číslo: **CVE-{YYYY}-{ID}**

Může mít i jméno, např. **BlueKeep**, **Eternal Blue**, **Spectre**, …
---
layout: default
---
# Hodnocení zranitelností — CVSS

Označuje závažnost zranitelnosti. Atributy:

- lokální vs. vzdálený přístup vs. fyzický
- interakce uživatele vs. není potřeba
- bez privilegií vs. potřeba privilegovaného uživatele

| Skóre | Závažnost |
|-------|-----------|
| 0 | None |
| 0.1–3.9 | Low |
| 4–6.9 | Medium |
| 7–8.9 | High |
| 9–10 | **Critical** |
---
layout: default
---
# Přehled zranitelností

<v-clicks>

- **Remote Code Execution (RCE)** – útočník spustí libovolný kód na cílovém systému
- **SQL Injection** – škodlivý SQL kód → neoprávněný přístup k databázi
- **Cross‑Site Scripting (XSS)** – vkládání škodlivých skriptů do webových stránek
- **Cross‑Site Request Forgery (CSRF)** – nutí uživatele provést nechtěnou akci
- **Privilege Escalation** – útočník získá vyšší oprávnění
- **Buffer Overflow** – přetečení bufferu → spuštění škodlivého kódu
- **Directory Traversal** – přístup k souborům mimo určený adresář
- **Insecure Deserialization** – manipulace s daty nebo spuštění kódu
- **Zero‑Day** – neznámá zranitelnost bez opravy
- **Broken Authentication** – slabé ověřování → převzetí účtů
- **Security Misconfiguration** – špatné nastavení otevírá cestu útokům

</v-clicks>
