
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
![Mall för MFA](./01_mall_val_MFA_admins.png)

---

### Bild 2 – Sammanfattning: Policy för risky sign-in
![Sammanfattning del 1](./02_sammanfattning_del1.png)

---

### Bild 3 – Sammanfattning: Roller och appar
![Sammanfattning del 2](./03_sammanfattning_del2_roller_appar.png)

---

## Dokumentation

Se nedan för fullständiga Word-filer för denna veckas labb:

- `SC300_Vecka3_Teori.docx` – Teori och bakgrund
- `SC300_Vecka3_Labb.docx` – Del 1: Skapa policy med MFA
- `SC300_Vecka3_Labb_Del2.docx` – Del 2: Risk-based Conditional Access
- `SC300_Vecka3_Labb_Del3.docx` – Del 3: App-specifik policy

---

## Viktiga lärdomar

- Rapportläge möjliggör säker testning av policys innan full tillämpning.
- Riskbaserade CA-policys ökar säkerheten utan att störa alla användare.
- Policytilldelning kan ske baserat på roller, appar och risknivåer.
