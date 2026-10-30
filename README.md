# 🍽️ Middagslogg

En enkel app for mobilen for å logge middagene dere spiser, registrere hvilke varer hver middag trenger,
og lage en samlet handleliste for en hel uke eller måned.

## Funksjoner

- **Logg** – registrer dato og middag (navn foreslås fra tidligere middager).
- **Middager** – legg til varer (mengde, enhet og butikkavdeling) og notater/oppskrift for hver middag.
  Viser hvor ofte hver middag er spist.
- **Handleliste** – velg siste uke, siste 30 dager eller en egen periode. Varene fra alle middagene i
  perioden summeres (g/kg og ml/dl/l slås sammen) og grupperes etter avdeling. Juster antall per middag,
  eller gang hele perioden opp, for å planlegge neste måned. Kryss av det du har hjemme, og kopier eller del listen.
- **Data** – last ned og gjenopprett backup (JSON).

Appen er én statisk nettside (`index.html`) som fungerer offline og kan legges til på hjem-skjermen.
Dataene lagres lokalt på telefonen, i nettleseren – ta backup jevnlig.

## Ta i bruk på telefonen

1. Publiser med GitHub Pages: **Settings → Pages → Build and deployment → Deploy from a branch**,
   velg grenen og mappen `/ (root)`.
2. Åpne adressen (`https://<brukernavn>.github.io/<repo>/`) på telefonen.
3. **iPhone:** Safari → Del → «Legg til på Hjem-skjerm». **Android:** Chrome → ⋮ → «Installer app».

## Kjøre lokalt

```
python3 -m http.server 8000
```

Åpne deretter http://localhost:8000.
