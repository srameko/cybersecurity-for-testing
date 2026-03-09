---
layout: section
---
# Zranitelnosti
---
layout: default
---
# Životní cyklus zranitelnosti


1. **Objev** — najdete zranitelnost
2. **Report výrobci** (Bug bounty)
3. **Potvrzení + odměna**
4. **Oprava za 30–90 dní** (update / patch)


<img src="/cve-2020-2555.png" class="mx-auto mt-4" style="max-height: 45%; width: 70%; object-fit: contain;" />
---
layout: default
---
# Označení zranitelnosti — CVE

<div class="grid grid-cols-2 gap-8 mt-2">
<div>

Po ověření je přiřazeno číslo: **CVE-{YYYY}-{ID}**

Může mít i jméno, např. **BlueKeep**, **Eternal Blue**, **Spectre**, …

</div>
<div>

<img src="/cve-2019-0708.png" style="object-fit: contain; max-height: 100%;" />

</div>
</div>
---
layout: default
---
# Hodnocení zranitelností — CVSS

<div class="grid grid-cols-2 gap-8 mt-2">
<div>

Označuje závažnost zranitelnosti. Atributy:

- lokální vs. vzdálený přístup vs. fyzický
- interakce uživatele vs. není potřeba
- bez privilegií vs. potřeba privilegovaného uživatele

</div>
<div>

<table class="w-full mt-2">
  <thead>
    <tr><th class="text-left">Skóre</th><th class="text-left">Závažnost</th></tr>
  </thead>
  <tbody>
    <tr><td>0</td><td class="text-gray-400 font-semibold">None</td></tr>
    <tr><td>0.1–3.9</td><td class="text-green-500 font-semibold">Low</td></tr>
    <tr><td>4–6.9</td><td class="text-yellow-500 font-semibold">Medium</td></tr>
    <tr><td>7–8.9</td><td class="text-orange-500 font-semibold">High</td></tr>
    <tr><td>9–10</td><td class="text-red-600 font-bold">Critical</td></tr>
  </tbody>
</table>

</div>
</div>
---
layout: default
---
# Přehled zranitelností


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

