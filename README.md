# Ordjagt

En lille web-app hvor børn på 5–10 år lærer engelske ord.

**Prøv den:** https://BRUGERNAVN.github.io/ordjagt/

## Sådan virker den

Barnet går gennem ni baner med i alt 72 engelske hverdagsord. Hver bane har to
dele: først vises ordene ét ad gangen med billede og udtale, derefter er der en
leg, hvor barnet hører et ord og trykker på det rigtige billede.

Et rigtigt svar giver farveglimt, konfetti og en glad lyd. Et forkert svar giver
ingen straf — feltet falmer, ordet siges igen, og efter to forsøg vises det
rigtige svar med en grøn kant. Hver klaret bane giver 1–3 stjerner og åbner den
næste.

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
