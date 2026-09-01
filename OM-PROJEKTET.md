# Ordjagt — hvad det er, og hvor tingene ligger

Skrevet 1. september 2026. Læs det her først, hvis du vender tilbage efter en pause.

## Idéen

En app hvor børn på 5–10 år lærer engelsk. Målet er ikke gloser til en prøve,
men **almindelige hverdagsord, man faktisk skal bruge for at snakke med nogen,
der kun kan engelsk.**

Barnet rejser gennem et middelalderrige med ni stationer: Skovlysningen,
Landsbyen, Kroen, Stenbroen, Troldehulen, Bjergpasset, Den gamle ruin,
Slotsporten og til sidst Dragetårnet, hvor prinsessen bliver befriet. En ridder
går ad stien og rykker videre, hver gang et sted er klaret. Steder man ikke har
nået, ligger i tåge.

## Sådan virker et sted

**Først lær:** stedets otte ord vises ét ad gangen. Stort billede, det engelske
ord, det danske ord nedenunder, og telefonen læser ordet højt. Barnet kan trykke
for at høre igen.

**Så leg:** barnet hører et engelsk ord og trykker på det rigtige af fire
billeder. Kun billeder — aldrig dansk tekst i legen, så barnet kobler lyden
direkte til tingen.

**Rigtigt svar:** guldglimt, konfetti, glad lyd.
**Forkert svar:** ingen straf. Feltet bliver rødt med et kryds, ordet siges igen.
Efter to fejl begynder det rigtige svar at banke med grøn kant, så ingen sidder
fast.

**Klaret sted:** skattekiste med 1–3 guldmønter, og næste sted låses op. Man kan
altid gå tilbage og tage et sted om for at få alle tre mønter.

72 ord i alt, otte pr. sted: følelser, mennesker, farver, tal, dyr, mad, krop og
tøj, hjemmet, udenfor.

## Beslutninger vi traf, og hvorfor

**Web-app frem for rigtig app.** Kan afprøves med det samme på enhver telefon,
uden App Store, uden udviklerkonto til 700 kr/år. Kan pakkes om til en rigtig app
senere — arbejdet er ikke spildt.

**Ingen login, ingen reklamer, ingen køb, intet tidspres.** En femårig kan ikke
logge ind, og et barn skal ikke mødes af noget, der vil have penge.

**Appen kontakter ingenting på nettet.** Google Fonts blev fjernet undervejs,
fordi den sender barnets IP-adresse til Google — det har givet bøder i EU. Nu
bruges telefonens egne skrifter. Ingen sporing, ingen cookies, ingen data der
forlader telefonen. Fremskridt gemmes lokalt i browseren.

**Al grafik er tegnet fra bunden i kode.** Intet hentet, intet kalkeret. Emoji er
Unicode-tegn, som telefonen selv tegner — derfor ingen billedrettigheder.

**Udtalen kommer fra telefonens indbyggede oplæser.** Gratis, virker for alle ord,
og nye ord kræver ingen optagelser.

## Hvad barnet sagde (den rigtige test)

To ting kom frem, da et barn prøvede den, og begge er rettet:

1. Billederne var for tvetydige — "thank you" som en gavepakke kunne ikke gættes.
   De ord er skiftet ud, og det danske ord er tilføjet på lær-kortene.
2. Forkert svar var for usynligt. Nu bliver feltet rødt med et stort kryds.

## Hvor tingene ligger

- **Kode på din Mac:** `/Users/danielandersen/claude code /ordjagt/`
  (mappen har et mellemrum til sidst i "claude code " — det driller, hvis stien
  ikke er i anførselstegn)
- **Live på nettet:** https://leinadnesredna.github.io/ordjagt/
- **Koden på GitHub:** https://github.com/leinadnesredna/ordjagt
- **Privat version hos Claude:** claude.ai/code/artifact/07c660c8-32e0-4133-8e6c-1260c524dc66

Hele appen er **én fil**, `index.html`. Der er ingen byggeproces og intet at
installere.

## Sådan opdaterer du den

Ændringer sendes op med `git push` fra `ordjagt`-mappen, og GitHub lægger dem
automatisk på hjemmesiden efter et par minutter.

Nøglen der giver adgang, ligger i din Macs nøglering og **udløber 26. september
2026.** Når git en dag begynder at spørge om adgangskode, er det bare den, der er
udløbet. Så laver du en ny på github.com/settings/tokens — kun adgang til
`ordjagt`, kun **Contents: Read and write** — og indsætter den, når den spørger.
Skriv den aldrig ind i en chat.

## Hvad der mangler — vigtigst først

**1. Repetition.** Det største hul. Ordene kommer aldrig igen, når et sted er
klaret, og sådan husker hjernen ikke. Løsningen: hvert sted starter med to ord
fra tidligere steder, plus et sted der blander alt det, barnet har lært. Det er
her, der er mest at hente.

**2. Kun én slags opgave.** Barnet hører engelsk og vælger et billede — men bliver
aldrig spurgt den anden vej. Vi ved ikke, om det selv kan komme i tanke om ordet.

**3. Lær-fasen kan ikke springes over,** heller ikke når man tager et sted om for
tredje gang. Det er dér, jeg ville forvente, at et barn falder fra.

**4. Appen dør stille, hvis telefonen mangler en engelsk stemme** — det sker på
nogle Android-telefoner. Den burde opdage det og sige det.

**5. Fremskridt kan forsvinde.** Det ligger kun i browseren. Ryddes browserdata
eller skiftes telefon, er alt guldet væk uden varsel.

**6. Virker ikke offline endnu.** Filen gør, men adressen skal hentes over nettet.

## Det med grafikken

Grafikken er tegnet i kode, og det betyder rene, flade former. Ønsket var en
malet tegneserie-baggrund i stil med 2000'ernes børne-tv, og det kan kode ikke
levere — malet grafik er malet, ikke geometri.

Planen, hvis du vil derhen: generér billederne selv (fx i ChatGPT) ud fra
art style-guiden, gem dem som PNG med gennemsigtig baggrund i en mappe
`billeder/` inde i `ordjagt`, og få dem bygget ind. Der ligger en færdig prompt
til det i samtalen fra 1. september 2026.

Juridisk tommelfingerregel, uanset hvad: beskriv **teknikken** ("tyk kontur,
flade farver, cel-shading"), aldrig en navngiven serie, figur eller studie. Stil
kan ingen eje. Figurer kan.
