# Joie BeLux Store Locator

Deze website is een eenvoudige, tweetalige store locator voor Joie-verkooppunten in België en Luxemburg.

De website helpt bezoekers om snel een verkooppunt, Google Maps-route of webshop te vinden.

## Pagina’s

- `index.html` — Nederlandstalige store locator
- `index-fr.html` — Franstalige store locator
- `info.html` / `info-fr.html` — wettelijke informatie
- `privacy.html` / `privacy-fr.html` — privacybeleid
- `cookies.html` / `cookies-fr.html` — cookiebeleid
- `openstreetmap.html` / `openstreetmap-fr.html` — informatie over OpenStreetMap en Nominatim

## Winkeldata

De verkooppunten worden ingeladen via JSON-bestanden:

- `stores.json`
- `stores-nl.json`
- `stores-fr.json`

De winkeldata bevat onder andere:

- winkelnaam
- adres
- postcode
- stad
- land
- website of webshop
- Google Maps-link
- coördinaten
- taalvelden voor Nederlands en Frans

De data kan worden beheerd via een gekoppelde spreadsheet en daarna worden omgezet naar JSON.

## Functionaliteiten

De website bevat:

- Nederlandstalige en Franstalige versie
- zoekfunctie op plaats, stad of postcode
- knop om de huidige locatie te gebruiken
- sortering van winkels op afstand na een locatiezoekopdracht
- links naar Google Maps
- links naar webshops of websites van verkooppunten
- juridische, privacy- en cookiepagina’s

## Privacy

De huidige versie gebruikt geen Meta Pixel, Google Analytics of marketingcookies.

De locatie van de bezoeker wordt enkel gebruikt na toestemming van de browser en dient alleen om winkels op afstand te sorteren.

## Externe diensten

De website kan gebruikmaken van:

- Google Maps voor route- en winkelverwijzingen
- OpenStreetMap en Nominatim voor locatieherkenning
- externe websites of webshops van verkooppunten

## Hosting

Voor officieel gebruik wordt aanbevolen om de website te plaatsen onder een officiële domeinnaam of hostingomgeving van Bomedys.

Voorgestelde domeinnaam:

`joiebaby-stores-belux.be`

## Professionele versie

Deze versie bevat de belangrijkste productiecorrecties:

- geen dubbele plaatsnamen meer op de kaart; de handmatige city-label-laag is verwijderd
- de Leaflet-prefix is uit de kaartvermelding gehaald
- de verplichte zichtbare bronvermelding voor OpenStreetMap contributors en CARTO blijft op de kaart staan
- juridische, privacy-, cookie- en OpenStreetMap-pagina’s zijn datumconsistent gemaakt
- privacy- en cookiepagina’s vermelden ook externe kaart/CDN-bronnen
- lege spreadsheetkolommen zoals `Unnamed: ...` worden niet meer opgenomen in de JSON-export
- inline `onclick`-handlers op de hoofdpagina’s zijn vervangen door JavaScript event listeners
- externe links uit de winkeldata worden beperkt tot `http`- en `https`-links

Belangrijk voor definitieve publicatie: controleer bij verhuis naar een officiële Joie- of Bomedys-hostingomgeving of de privacytekst nog exact overeenkomt met de werkelijke hosting en gebruikte externe diensten.

