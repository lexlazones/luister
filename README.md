# luister.

Eerste testversie van een eenvoudige, rustige, kindvriendelijke luisterinterface (PWA).

## Testen
- Open de GitHub Pages-site op een iPhone in Safari.
- Deel > Zet op beginscherm.
- Afspelen produceert zelf gegenereerde, zachte testtonen (geen Spotify of luisterboeken).
- Open ouderinstellingen met de voorlopige pincode `1234` en wijzig deze direct.
- Zet op iPhone **Begeleide toegang** aan om de app niet te kunnen verlaten.

## Belangrijke beperkingen
- De ouderpincode is een eenvoudige interfacebarrière, **geen veilige authenticatie**: instellingen staan lokaal in de browser. Gebruik geen vertrouwelijke gegevens.
- Geluiden zijn alleen technische placeholders. De originele .wav-bestanden uit de offline demo zijn hier bewust niet nodig.
- De slaaptimer loopt zolang de browserpagina actief is; iOS kan web-apps op de achtergrond onderbreken.
- Geen Spotify-integratie. Kindgerichte Spotify-apps kunnen beperkt zijn door Spotify's ontwikkelaarsvoorwaarden.
- SVG als icoon wordt niet door alle iOS-versies als beginscherm-icoon ondersteund. Een PNG-icoon is een latere verbetering.

## Bestanden
`index.html` (app), `manifest.webmanifest` (installatie), `sw.js` (offline), `icon.svg` (voorlopig logo).
