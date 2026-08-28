# Ordjagt

En lille web-app hvor børn på 5–10 år lærer engelske ord.

**Prøv den:** https://leinadnesredna.github.io/ordjagt/

## Sådan virker den

Appen er et søkort med ni øer og i alt 72 engelske hverdagsord. Barnet sejler
fra ø til ø: først vises øens ord ét ad gangen med billede, udtale og det danske
ord, derefter er der en leg, hvor barnet hører et ord og trykker på det rigtige
billede. Klarer man øen, åbner en skattekiste, og skibet sejler videre til den
næste ø.

Et rigtigt svar giver guldglimt, konfetti og en glad lyd. Et forkert svar giver
ingen straf — feltet bliver rødt med et kryds, ordet siges igen, og efter to
forsøg begynder det rigtige svar at banke med en grøn kant. Hver klaret ø giver
1–3 guldmønter.

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
