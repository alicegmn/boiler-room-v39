Kontaktformulär:
Flödesschema: https://miro.com/app/board/uXjVLbE_njU=/?share_link_id=855890900924

1. Användarens handling:
Användaren fyller i kontaktformuläret (namn, e-post, meddelande) och klickar på "Skicka" eller motsvarande knapp.

2. Frontend-komponenter:
När användaren klickar på "Skicka" skickas data från formuläret (HTML och JavaScript hanterar detta). Formulärets validering sker lokalt (JavaScript kollar om fälten är ifyllda korrekt, t.ex. om e-post har rätt format). Formuläret och sidan den befinner sig på är troligtvis stylead, med CSS.

3. Kommunikation med backend:
Om valideringen är godkänd, skickas formulärdata via ett API-anrop (HTTP POST-begäran) till backend-servern. Här används vanligtvis AJAX eller fetch() i JavaScript för att kommunicera med servern utan att ladda om sidan.

4. Backend-processer:
Mottagning av data: Servern (t.ex. Node.js, PHP, Python) tar emot API-anropet med formulärdata.
Validering: Backend validerar data igen för säkerhet och korrekthet (t.ex. att e-post är unik eller att inga fält är tomma).
Databashantering: Om valideringen går igenom, sparas informationen i databasen (t.ex. MySQL, MongoDB).
Respons genereras: Backend skapar en JSON-respons som skickas tillbaka till frontend. Denna respons kan innehålla framgångsmeddelanden, felmeddelanden eller annan relevant information.

5. Frontend-uppdatering:
Frontend tar emot JSON-responsen och uppdaterar gränssnittet:
Vid framgång: Ett tackmeddelande visas för användaren och formuläret kan rensas.
Vid fel: Ett felmeddelande visas, t.ex. att vissa fält saknar korrekt data eller att det uppstod ett problem med servern.

-----

DOKUMENTATION:
- Mycket fika och gött snack i gruppen!

Anton:
- Dundrade igång och gjorde 3 cards för att testa så att det funkade som jag tänkte med grid, det fick fint!
- Snubblade lite med flexbox inom cardsen, glömde tänka och jobbade med fel parent/child väldigt länge innan jag kollade på html:en och löste det.
- Hade lite problem att bli kompis med clamp. Vi är inte vänner än, men iaf inte ovänner.

Rhiannon: 
- made a photo gallery page using Grid
- used aria-labels as alt-text for images
- used clamp() for the text overlay 
- used overlay to make the text easier to read by increasing the contrast between text and background 
- used media queries to remove some of the images when the screen becomes smaller

Alice:
