# Week 5 – External Identities (B2B & Federation)

## 🎯 Syfte
I denna labb undersöktes hur man arbetar med **External Identities (B2B)** i Microsoft Entra ID. Fokus låg på att bjuda in externa användare, verifiera deras åtkomst, samt hantera grupper och rolltilldelningar.

---

## 📑 Steg 1 – Bjud in extern användare
En ny B2B-användare bjuds in via **Entra ID → Users → New guest user**.

![01_b2b_invitation](week5_screenshots_fixed/01_b2b_invitation.png)

---

## 📑 Steg 2 – Gästanvändare skapad
Efter inbjudan syns gästanvändaren i användarlistan.

![02_b2b_user_created](week5_screenshots_fixed/02_b2b_user_created.png)

---

## 📑 Steg 3 – Inbjudningsmejl
Den externa användaren får ett mejl med länk för att acceptera inbjudan.

![03_invitation_email](week5_screenshots_fixed/03_invitation_email.png)

---

## 📑 Steg 4 – Skapa grupp för B2B
En ny säkerhetsgrupp skapas för att organisera externa användare.

### Fält ifyllda:
![04_group_creation_step1](week5_screenshots_fixed/04_group_creation_step1.png)

### Ägare och medlem vald:
![05_group_creation_step2](week5_screenshots_fixed/05_group_creation_step2.png)

### Bekräftelse vid skapande:
![06_group_creation_confirmation](week5_screenshots_fixed/06_group_creation_confirmation.png)

### Gruppens översikt (extra kontext):
![04b_group_overview](week5_screenshots_fixed/04b_group_overview.png)

---

## 📑 Steg 5 – Verifiering
Gruppen tilldelas en roll (Reader) på resursgruppen i Azure. Detta bekräftar att B2B-användaren nu har åtkomst via gruppen.

![07_verification_result](week5_screenshots_fixed/07_verification_result.png)

---

## ✅ Slutsats
- Externa användare kan bjudas in och verifieras via B2B-inbjudan.  
- Gästanvändare hanteras smidigt via grupper för åtkomstkontroll.  
- Rolltilldelningar fungerar även för externa identiteter.  

Denna labb visar på hur **External Identities** kan användas för att på ett säkert sätt samarbeta med externa parter.
