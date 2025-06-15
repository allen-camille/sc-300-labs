# SC-300 – Vecka 3: Conditional Access & MFA – Del 2
I detta moment skapades en princip för villkorsstyrd åtkomst baserat på riskfyllda inloggningar.
Principens namn: 'Kräv MFA vid risky sign-in'

Steg som genomfördes:
1. Alla användare inkluderades i tilldelningen.
2. Alla molnappar valdes som målresurser.
3. Ett villkor för risky sign-in valdes (t.ex. användare med 'sign-in risk' eller annan signal från Identity Protection).
4. Kontrollinställning: 'Kräv multifaktorsautentisering' valdes som åtgärd.
5. Principen sattes till 'Endast rapport' för att utvärdera effekten utan att påverka användarna direkt.
6. Varning om att utesluta administratör beaktades, men användaren valde att fortsätta ändå.

Denna princip loggas nu och kan ses i rapporter via Microsoft Entra.
Dokumentationsdatum: 2025-06-14 16:40