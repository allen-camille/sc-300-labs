
# SC-300 Week 3 – Conditional Access & MFA

## Sammanfattning

I denna vecka konfigurerades **Conditional Access-policys** i Microsoft Entra ID för att förstärka säkerheten vid inloggningar. Fokus låg på att kräva **Multifaktorautentisering (MFA)** vid riskfyllda sign-ins, och att använda **rapportläge** för att testa utan påverkan på användarna.

## Delmoment

1. Skapa policy som kräver MFA för administratörsroller.
2. Ange villkor: riskfylld inloggning (user risk).
3. Aktivera rapportläge och analysera sign-ins.
4. Skapa policy för appar som kräver MFA.
5. Reflektera kring säkerhetsvinster och användarpåverkan.

---

## Screenshots och beskrivningar

### Bild 1 – Mall för MFA-policy för administratörer
![Bild1](./01_mall_val_MFA_admins.png)

### Bild 2 – Sammanfattning: Policy för risky sign-in
![Bild2](./02_sammanfattning_del1.png)

### Bild 3 – Sammanfattning: Roller och appar
![Bild3](./03_sammanfattning_del2_roller_appar.png)

### Bild 4 – Principöversikt och meddelanden om skapade policies
![Bild4](./10dbf119-b30d-4c30-883a-0c92b181566c.png)

### Bild 5 – Bevilja MFA i princip (rapportläge)
![Bild5](./1f6c86a5-d186-4f89-a41e-b95c8f679df8.png)

### Bild 6 – Ej konfigurerat nätverk och aktivering i rapportläge
![Bild6](./2567e32f-d975-4023-9f5e-3567deb60d82.png)

### Bild 7 – Princip från mallar med valda roller och appar
![Bild7](./4bb5c573-711c-4998-b434-30cce036a20e.png)

### Bild 8 – Bekräftelse av påverkan vid policyaktivering
![Bild8](./8d07abdf-3630-4e6b-9f0b-e7f4c9ecc234.png)

### Bild 9 – Blockera åtkomst vid hög användarrisk
![Bild9](./ab7e86b9-32e5-4f8e-8c3e-25686b2f4994.png)

---

## 📘 Läs direkt i GitHub

- [SC300_Vecka3_Teori.md](./SC300_Vecka3_Teori.md) – Teori och bakgrund
- [SC300_Vecka3_Labb.md](./SC300_Vecka3_Labb.md) – Del 1: Skapa policy med MFA
- [SC300_Vecka3_Labb_Del2.md](./SC300_Vecka3_Labb_Del2.md) – Del 2: Risk-based Conditional Access
- [SC300_Vecka3_Labb_Del3.md](./SC300_Vecka3_Labb_Del3.md) – Del 3: App-specifik policy

---

## Viktiga lärdomar

- Rapportläge möjliggör säker testning av policys innan full tillämpning.
- Riskbaserade CA-policys ökar säkerheten utan att störa alla användare.
- Policytilldelning kan ske baserat på roller, appar och risknivåer.
