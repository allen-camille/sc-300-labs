# SC-300 – Vecka 3: Conditional Access & MFA – Labbdokumentation
## 🔹 Del 1 – Skapa MFA-policy för administratörer
En Conditional Access-policy skapades med målet att kräva multifaktorautentisering (MFA) för användare med administratörsroller.

🧭 Steg:
1. Gå till Microsoft Entra Portal > Skydd > Villkorsstyrd åtkomst
2. Välj 'Skapa ny princip från mallar'
3. Välj mallen: 'Kräv multifaktorauthentisering för administratörer'
4. Klicka på 'Granska och skapa'
5. Principens status sattes till: 'Endast rapportläge' (för att undvika skarp påverkan vid test)
6. Roller som omfattades inkluderade bl.a.: Global administratör, Användaradministratör, Säkerhetsadministratör m.fl.
7. Policyn gäller för alla molnappar och kräver MFA som åtkomstkontroll
8. Principen sparades och aktiverades i rapportläge