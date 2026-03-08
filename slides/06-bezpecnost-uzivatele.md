---
layout: section
---
# Bezpečnost pro uživatele
## To nejdůležitější, co byste měly vědět

---
layout: default
---
# Jak začít s osobní bezpečností?

Ty nejdůležitější zvyky, které vám v dlouhodobém horizontu usnadní život.

---
layout: default
---
# Aktualizujte!

| Co | Kdy |
|---|---|
| Windows | Každé druhé úterý v měsíci |
| Apple | Zpravidla co dva měsíce, někdy i častěji |
| Oracle | Čtvrtletně |
| Aplikace (Chrome, Firefox, …) | Ad Hoc, dle release cyklu |
| Firmware (BIOS, router, žárovka, …) | Dle dostupnosti |

> Aktualizace opravují chyby, které útočníci aktivně zneužívají.

---
layout: default
---
# Ochrana před škodlivým kódem

**Antivir:**

- Windows 10+: klidně použijte vestavěný **Defender**
- macOS: nemá vestavěný AV — zvažte Eset, Avast, AVG, Bitdefender, Intego
- Nezapomínejte na **mobilní zařízení (Android)**

**Pravidelné testování** + testování na vyžádání

---
layout: default
---
# Základní zabezpečení počítače

**Zamknutí obrazovky:**

| OS | Zkratka |
|---|---|
| Windows | `Win + L` |
| Linux | `Ctrl + Alt + L` nebo `Super + L` |
| macOS | `Control + Command + Q` |

**Least privilege:**
- Nepoužívejte účet s administrátorským oprávněním
- Nastavte si heslo: 13+ znaků (malé, velké, čísla), ideálně frázové

---
layout: default
---
# Přihlašování a hesla

<v-clicks>

- **Nastavte si MFA (2FA)**, nejlépe Passkeys — sociální sítě, e-mail, banka, …
- **Co služba, to unikátní heslo** — ověřte na [haveibeenpwned.com](https://haveibeenpwned.com)
- **Správce hesel** — pamatujete si jen jedno heslo (1Password, BitWarden, …)
- **SSO** — [mojeid.cz](https://www.mojeid.cz), [bankid.cz](https://www.bankid.cz/), Apple / Google / Facebook

</v-clicks>

---
layout: default
---
# Základní pravidla zálohování

**Pravidlo 3-2-1:**

| | |
|---|---|
| **3** | Tři kopie dat |
| **2** | Dvě fyzicky nezávislá úložiště |
| **1** | Jedna kopie offsite (mimo budovu) |

- Pravidelnost: jednou denně, týdně, … (co je pro vás proveditelné)
- Zálohu **chraňte heslem!**

---
layout: default
---
# Šifrování disku

**Šifrujte** — při ztrátě zařízení nejsou data ohrožena:

| OS | Nástroj |
|---|---|
| Windows | BitLocker |
| Linux | LUKS |
| macOS | FileVault |
| iOS / Android | Vestavěné šifrování |

---
layout: default
---
# Co mám dělat když měním zařízení?

**Prodávám počítač / telefon:**

| Zařízení | Postup |
|---|---|
| PC (šifrovaný) | Uvést do továrního nastavení |
| PC (nešifrovaný) | Zformátovat |
| Telefon | Tovární nastavení |

**Zbavuju se zařízení (fyzicky):**

| Zařízení | Postup |
|---|---|
| PC | Vytáhnout a zničit disk (kladivo) |
| Telefon | Vytáhnout paměťovou kartu a zničit (nůžky) |

> Nezapomenout na SIM!
