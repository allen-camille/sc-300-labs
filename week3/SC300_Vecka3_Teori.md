# SC-300 – Vecka 3: Access Management – Teori
## 🛡️ Privileged Access och PIM
Privileged Identity Management (PIM) är en funktion i Microsoft Entra (Azure AD) som gör det möjligt att:
- Bevilja Just-in-Time (JIT) åtkomst till resurser
- Kräva godkännande innan aktivering
- Ställa in automatisk utloggning efter en viss tid
- Visa historik över privilegierad åtkomst

PIM används främst för att minimera risken med permanenta privilegierade roller som t.ex. Global administratör, User Administrator eller Security Reader.
## 🧩 Rolltyper i Azure AD
## ⏱️ Just-In-Time Access (JIT)
- Tillfällig aktivering av roller istället för permanent tilldelning
- Kräver förklaring, MFA, och/eller godkännande
- Kan schemaläggas eller begäras manuellt via PIM
## ✅ Godkännanden
- Kan aktiveras så att en viss person eller grupp måste godkänna innan åtkomst beviljas
- Skapar kontroll och insyn över privilegierad åtkomst
## 🧾 Åtkomstgranskning och historik
PIM erbjuder:
- Loggning av alla aktiveringar/deaktiveringar
- Visning av tidigare begärd åtkomst
- Export till Log Analytics eller Microsoft Sentinel
## 🎯 Nyttiga begrepp
