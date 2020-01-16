

# Bedömningsshandledning Webbserverprogrammering 1

## Matris

| Aspekt         | E                                                            | C                                                            | A                                                            |
| -------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Dokumentation  | Tillsammans med läraren dokumenterar du **översiktligt** din applikations funktionalitet, utvecklingsprocess och säkerhet och använder **med viss säkerhet *enkel*** terminologi. | Med läraren som bollplank dokumenterar du **utförligt** din applikations funktionalitet, utvecklingsprocess och säkerhet och använder **med viss säkerhet** ***korrekt*** terminologi. | Med läraren som bollplank dokumenterar du **utförligt  och nyanserat** din applikations funktionalitet, utvecklingsprocess och säkerhet och **använder med säkerhet *korrekt*** terminologi. |
| Arkitektur     | Tillsammans med läraren utvecklar du en applikation där koden har en **enkel** kodstruktur. | Med läraren som bollplank utvecklar du en applikation där koden har en **god** kodstruktur. | Med läraren som bollplank utvecklar du en applikation där koden **följer MVC** och **följer en given kodstandard.** |
| Funktionalitet | Tillsammans med läraren  utvecklar du en applikation med **enkel** funktionalitet. | Med läraren som bollplank utvecklar du en applikation med **inloggningssystem** och **tillfredsställande** funktionalitet. | Med läraren som bollplank utvecklar du en applikation med ett **inloggningssystem** och **komplex** funktionalitet. |
| Datalagring    | Tillsammans med läraren  utvecklar du en applikation som använder en **enkel** lösning för att spara data mellan sidvisningar. | Med läraren som bollplank utvecklar du en applikation som använder en e**nkel databaslösning** för att spara data mellan sidvisningar. | Med läraren som bollplank utvecklar du en applikation som använder en **komplex databaslösning** för att spara data mellan sidvisningar. |
| Säkerhet       | Tillsammans med läraren vidtar du **enkla** åtgärder för att förhindra att applikationen utnyttjas. | Med läraren som bollplank vidtar du **lite mer avancerade** åtgärder för att förhindra att applikationen utnyttjas. | Med läraren som bollplank vidtar du **avancerade** åtgärder för att förhindra att applikationen utnyttjas. |

### E-nivå

Gemensamt för samtliga aspekter på E-nivå är en brist på självständighet. Detta innebär att den efterfågade funktionaliteten i aspekterna nedan kan till viss del tagits fram tillsammans med läraren.

### C-nivå

Gemensamt för samtliga aspekter på C-nivå är större grad av självständighet än på E-nivå.

### A-nivå

Gemensamt för samtliga aspekter på A-nivå är en större grad av självständighet än på E-nivå.

## Dokumentation
| E                                                            | C                                                            | A                                                            |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Tillsammans med läraren dokumenterar du **översiktligt** din applikations funktionalitet, utvecklingsprocess och säkerhet och använder **med viss säkerhet \*enkel\*** terminologi. | Med läraren som bollplank dokumenterar du **utförligt** din applikations funktionalitet, utvecklingsprocess och säkerhet och använder **med viss säkerhet** ***korrekt\*** terminologi. | Med läraren som bollplank dokumenterar du **utförligt  och nyanserat** din applikations funktionalitet, utvecklingsprocess och säkerhet och **använder med säkerhet \*korrekt\*** terminologi. |

### E-nivå

Eleven har en enkel beskrivning över applikationens funktionalitet (en enkel domänbeskrivning) och ett enkelt er-diagram. Eleven har svårt för begrepp som t.ex *route*, *resurs*, *vy*, *entitet*.

### C-nivå

Eleven har utförlig domänbeskrivning som beskriver olika användares behörigheter, och ett korrekt er-diagram. Eleven har svårt för mer avancerade begrepp som *RESTFUL* och *kardinalitet*.

### A-nivå

Eleven har domänbeskrivning likt C-nivå, och använder obehinrdat de flesta begrepp. Applikationens routes är även dokumenterade enligt tex Yardoc.

## Arkitektur

| E                                                            | C                                                            | A                                                            |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Tillsammans med läraren utvecklar du en applikation där koden har en **enkel** kodstruktur. | Med läraren som bollplank utvecklar du en applikation där koden har en **god** kodstruktur. | Med läraren som bollplank utvecklar du en applikation där koden **följer MVC** och **följer en given kodstandard.** |

### E-nivå

Eleven har i stort sett all logik i `app.rb`,.

Eleven kan upprepa logik som t.ex databasuppkopplingar och valideringar i flera routes snarare än använda `before-block`.

Elevens vyer/routes följer ingen tydlig namngivning

### C-nivå

Eleven har god separation av olika sorters logik.

Eleven har t.ex helper-funktioner för db-uppkoppling, använder before-block och har en någotsånär DRY-kod.

Eleven följer någotsånär REST och har en tydlig namngivning av vyer/routes.

### A-nivå

Eleven följer MVC (där det är möjligt att controllern bara består av en app.rb - men det är även möjligt att dela upp den efter resurs.)

Eleven följer REST fullt ut.

## Funktionalitet

| E                                                            | C                                                            | A                                                            |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Tillsammans med läraren  utvecklar du en applikation med **enkel** funktionalitet. | Med läraren som bollplank utvecklar du en applikation med **inloggningssystem** och **tillfredsställande** funktionalitet. | Med läraren som bollplank utvecklar du en applikation med ett **inloggningssystem** och **komplex** funktionalitet. |

### E-nivå

Applikationen erbjuder ett enkelt CRUD-gränssnitt (åtminstone Create/Show/Delete) för någon resurs. 

### C-nivå

Applikationen erbjuder ett enkelt CRUD-gränssnitt för några resurser, varav minst en har en association/relation till en annan resurs. 

Appliktionen har ett inloggninssystem, och det finns skillnad på vad man kan göra beroende på om man är inloggad eller ej.

### A-nivå

Applikationen erbjuder ett CRUD-gränssnit för flera resurser, där flera har associationer/relationer till varandra. Vid uppdatering och borttagning av relaterade resurser förändras även kopplade resurser där så är nödvändigt (t.ex genom `ON DELETE CASCADE`-liknande funktinalitet).

Inloggningssystemet skiljer på vad oinloggade och inloggade användare kan göra, och implementerar ett enkelt behörighetssystem (t.ex guest-user, standard-user, admin).

Eleven använder automatiserade tester (capybara) för att testa någon funktionalitet i applikationen.

## Datalagring

| E                                                            | C                                                            | A                                                            |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Tillsammans med läraren  utvecklar du en applikation som använder en **enkel** lösning för att spara data mellan sidvisningar. | Med läraren som bollplank utvecklar du en applikation som använder en e**nkel databaslösning** för att spara data mellan sidvisningar. | Med läraren som bollplank utvecklar du en applikation som använder en **komplex databaslösning** för att spara data mellan sidvisningar. |

### E-nivå

Eleven har en databas med minst en, korrekt formaterad, tabell (eller eventuellt, i nödfall, enbart sessioner)

### C-nivå

Eleven har en databas med flera tabeller, varav minst två har relationer med varandra

### A-nivå

Eleven har en databas med flera tabeller, varav minst två beskriver ett många-till-många-förhållande. Eftersom detta är omöjligt har eleven omvandlat det till två en-till-många via en relationstabell.

## Säkerhet

| E                                                            | C                                                            | A                                                            |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Tillsammans med läraren vidtar du **enkla** åtgärder för att förhindra att applikationen utnyttjas. | Med läraren som bollplank vidtar du **lite mer avancerade** åtgärder för att förhindra att applikationen utnyttjas. | Med läraren som bollplank vidtar du **avancerade** åtgärder för att förhindra att applikationen utnyttjas. |

### E-nivå

Om eleven har ett inloggningssystem kontrollerar hen användarnamn/lösenord (eventuellt hårdkodade).

Om eleven har ett inloggningssystem kontrollerar hen åtminstone någon get-route.

### C-nivå

Eleven har ett inloggningssystem, med hashade lösenord i databasen. Eleven säkrar upp routes (både `get` och `post` (både inloggning och att användaren "äger" resursen)

Eleven validerar och escapar användarinput

### A-nivå

Eleven har ett inloggninssystem med hashade lösenord i databasen. Eleven säkrar upp routes och implementerar t.ex logging kring inloggningsförsök och cool-down eller liknande vid hackningsförsök. Eventuellt implementerar eleven "strong params" mha black/whitelist.
Eleven kan även använda sig av Sinatras CSRF-funktionalitet
