# luister.

Eenvoudige, rustige luister-app (PWA) voor iPhone en Android. **Versie 0.5 is een prototype.**

## Starten

Open de [online app](https://lexlazones.github.io/luister/) op de iPhone. Gebruik Safari > Deel > Zet op beginscherm.

### Eigen verhalen (v0.5)

1. Tik op **Open mijn verhalen** op het startscherm.
2. Open het tandwiel en voer de voorlopige ouderpincode `1234` in (wijzig deze daarna).
3. Kies MP3, M4A, WAV of een ander op de iPhone ondersteund audiobestand via **Audio toevoegen**.
4. Sluit de ouderinstellingen en selecteer het verhaal.
5. Pauzeren, ±30 seconden spoelen en de slaaptimer zijn beschikbaar. De luisterpositie wordt lokaal opgeslagen.

De bestanden worden **niet naar GitHub of een server geüpload**: de PWA slaat ze in IndexedDB op het apparaat op. iOS kan lokale websiteopslag wissen onder bepaalde omstandigheden. Bewaar dus altijd je oorspronkelijke audiobestanden. De import is afhankelijk van beschikbare opslagruimte en de bestandsgrootte. Op andere apparaten verschijnen dezelfde bestanden niet automatisch. De import-, hervat- en achtergrond-audiowerking zijn nog niet op een echte iPhone getest.

### Spotify

In ouderinstellingen staat een link naar [Spotify-laboratorium](https://lexlazones.github.io/luister/spotify-lab.html). Deze pagina bevat een officiële ingesloten Spotify-speler en is **uitsluitend bedoeld als technische test voor volwassenen**. Spotify's ontwikkelaarsvoorwaarden beperken kindgerichte integraties. De kindgerichte luisterboekspeler gebruikt daarom uitsluitend eigen toegestane audiobestanden. De Spotify-labpagina is niet via sterke authenticatie afgeschermd en mag niet als kinderslot worden beschouwd.

### Kinderslot

De pincode van de ouderinstellingen is een **eenvoudige interfacebeperking**, geen veilige authenticatie. Gebruik op iPhone **Instellingen > Toegankelijkheid > Begeleide toegang** om de app te beperken tot één scherm. Let op dat Begeleide toegang bij normale webnavigatie het openen van webpagina's niet per se blokkeert; test de instelling op het apparaat.

### Updates

De app wordt als statische website via GitHub Pages gepubliceerd. De service worker cachet bestanden voor offline gebruik; bij een update verschijnt een melding als de browser de nieuwe worker heeft opgehaald. Als een oude versie blijft hangen, open dan de site eenmaal in Safari en sluit/heropen de web-app.

## Technisch

Vanilla JavaScript, HTML5 Audio, IndexedDB, service worker en GitHub Pages. Geen backend of externe audiobibliotheek.
