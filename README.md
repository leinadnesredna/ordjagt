# Ordjagt

En lille web-app hvor børn på 5–10 år lærer engelske ord.

**Prøv den:** https://leinadnesredna.github.io/ordjagt/

## Sådan virker den

Appen er en rejse gennem et middelalderrige med ni stationer og i alt 72
engelske hverdagsord. Barnet starter i Skovlysningen og går ad stien gennem
Landsbyen, Kroen, Stenbroen, Troldehulen, Bjergpasset, Den gamle ruin og
Slotsporten, indtil ridderen til sidst når Dragetårnet og befrier prinsessen.

Hvert sted har to dele: først vises stedets ord ét ad gangen med billede,
udtale og det danske ord, derefter er der en leg, hvor barnet hører et ord og
trykker på det rigtige billede. Klarer man stedet, åbner en skattekiste, og
ridderen går videre til det næste sted.

Et rigtigt svar giver guldglimt, konfetti og en glad lyd. Et forkert svar giver
ingen straf — feltet bliver rødt med et kryds, ordet siges igen, og efter to
forsøg begynder det rigtige svar at banke med en grøn kant. Hvert klaret sted
giver 1-3 guldmønter.

## Teknisk

Én enkelt HTML-fil uden nogen form for afhængigheder.

- Ingen biblioteker, ingen byggeproces, intet at installere
- Ingen forbindelser til nettet — appen henter intet fra andre servere
- Ingen sporing, ingen cookies, ingen konto, ingen data der forlader enheden
- Fremskridt gemmes lokalt i browseren
- Udtalen kommer fra enhedens indbyggede taleoplæser
- Billederne er emoji, altså almindelige Unicode-tegn, som enheden selv tegner

## Kør den lokalt

Åbn `index.html` i en browser. Det er det hele.
