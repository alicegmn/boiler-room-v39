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

Alice
– Vi började fredagen med ett uppstartsmöte kl 9.00 där vi satte ramarna för projektet och satte en struktur för vår trellobräda och la in våra första uppgifter i backloggen. Vi delade upp uppgifter/roller/ansvarsområden.
Detta var särskilt bra för mig som inte kunde delta under förmiddagen då jag var på resande fot, jag kunde enkelt följa gruppens tankegångar i vår trello.
– Sedan hade vi en standup igen kl 10.30 då jag fick en ordentlig förståelse för vad de bestämt tidigare under morgonen och de andra uppdaterade om hur det hade gått hittills. Sedan fortsatte vi (alla utom jag) jobba tills vi möttes kl 13.00 på scandic och jag var med på länk. Vi körde återkommande standups under eftermiddagen för att stämma av hur det gick.
– Klockan 13.00 kunde jag sätta igång arbetet med att koda,vilket var att skapa en “about page” för den webbplats som vi skulle ta fram som var inriktad på fotboll. Jag valde att presentera redaktionen som jobbar med plattformen samt en annons om att de (vi) söker medarbetare.
– Först satte jag html-strukturen med semantiska och icke-semantiska element.
– Sedan vill jag göra sidan responsiv, helst utan att använda media queries
– Jag började att göra en gridstruktur och lite andra lösningar som jag inte blev nöjd med. Då bestämde jag mig för att skriva väldigt detaljerade prompts till chatgpt istället och tog hjälp den vägen.
– Det var ett arbetssätt som också gjorde att jag lärde mig sådant som jag inte hade lärt mig lika snabbt utan ai.
– Jag avslutade med att göra tillgänglighetsanalyser med Wave och Lighthouse för att se om jag missat något WCAG-krav.
– Sedan fick jag lite tid över så jag testade runt med lite interaktiva effekter med transition och 
