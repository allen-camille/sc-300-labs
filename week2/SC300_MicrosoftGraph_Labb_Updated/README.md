# SC300 Microsoft Graph Lab

## Sammanfattning
Denna labb visar steg för att konfigurera en Azure AD app med rätt API-behörigheter för Microsoft Graph, 
skapa token och göra anrop mot Microsoft Graph API med Postman.

## Steg i labben

1. Skapa en app-registrering i Azure AD.
2. Lägg till API-behörigheter, både delegat och program (t.ex. User.Read, User.Read.All).
3. Bevilja administratörsgodkännande för organisationen för programbehörigheter.
4. Skapa en klienthemlighet under "Certificates & secrets".
5. Använd Postman för att skapa en token via OAuth 2.0 klientuppgifter (client_credentials).
6. Testa att anropa Microsoft Graph API, t.ex. https://graph.microsoft.com/v1.0/users.
7. Felsök vanliga fel som behörighetsproblem och ogiltiga URL:er.
8. Bekräfta att anropet fungerar och få JSON med användardata.

## Viktiga lärdomar
- Skillnad mellan delegat- och programbehörigheter.
- Hur man beviljar administratörsgodkännande.
- Användning av Postman för API-tester med OAuth 2.0.
- Vanliga fel och hur man löser dem.

## Mappstruktur
- screenshots/: innehåller alla skärmbilder från labben.
- README.md: denna sammanfattning.

# SC-300 Microsoft Graph API Lab

Denna laboration visar hur man registrerar en app i Azure, ger rätt API-behörigheter och testar anrop mot Microsoft Graph API med Postman.

---

## Screenshots och beskrivningar

### Bild 1: Postman – GET-anrop mot Microsoft Graph API för att hämta användare med giltig Bearer-token
![Postman GET Microsoft Graph API](screenshots/bild1.png)  
Visar API-förfrågan och JSON-svar med användardata.

---

### Bild 2: Azure Portal – App-registreringens API-behörigheter  
![Azure API-behörigheter](screenshots/bild2.png)  
Här listas tillagda delegerade API-behörigheter för appen, User.Read visas som ej administratörsgodkänd.

---

### Bild 3: Azure Portal – Välj typ av API-behörigheter för applikationen  
![Azure API-behörighetstyp](screenshots/bild3.png)  
Val mellan delegerade behörigheter (användarnamn) och programbehörigheter (applikationsnamn).

---

### Bild 4: Azure Portal – Lista över möjliga delegerade behörigheter under Microsoft Graph API  
![Azure delegerade behörigheter](screenshots/bild4.png)  
Här väljs specifika behörigheter, t.ex. User.Read.All för full läsbehörighet på användarprofiler.

---

### Bild 5: Azure Portal – Administratörsgodkännande krävs för vissa API-behörigheter  
![Administratörsgodkännande](screenshots/bild5.png)  
Bekräftelse på att User.Read.All kräver administratörsmedgivande för att aktiveras.

---

### Bild 6: Azure Portal – Appens API-behörigheter efter administratörsgodkännande  
![Godkända API-behörigheter](screenshots/bild6.png)  
User.Read och User.Read.All är nu godkända och aktiva.

---

### Bild 7: Postman – POST-anrop för att hämta access token via client credentials grant  
![Postman token request](screenshots/bild7.png)  
Visar hur client_id, client_secret, scope och grant_type skickas i kroppen för att få token.

---

### Bild 8: Postman – Lyckat GET-anrop med token mot Microsoft Graph API  
![Postman lyckat API-anrop](screenshots/bild8.png)  
JSON-svar med flera användare bekräftar att behörigheterna fungerar korrekt.


---

### Bild 9: Azure Portal – Välj mellan delegerade och programbehörigheter  
![API-behörighetstyper](screenshots/da613de3-e3fb-4682-8815-039c4ace9825.png)  
Här visas valet mellan delegerade (inloggad användare) och programbehörigheter (tjänst utan inloggning).

---

### Bild 10: Azure Portal – Endast User.Read har lagts till  
![API-behörighet User.Read](screenshots/e930003a-7563-43de-ae40-793b8cf42e29.png)  
Illustrerar att bara `User.Read` har lagts till som delegerad behörighet, utan administratörsgodkännande.



# Sammanfattning

I denna labb skapade vi en app i Azure, lade till och administratörsgodkände API-behörigheter för Microsoft Graph, hämtade token via klientuppgifter och testade API-anrop i Postman.  
Det visade hur man arbetar med OAuth 2.0 client credentials flow och Microsoft Graph API.
