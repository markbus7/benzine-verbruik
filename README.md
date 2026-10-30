# benzine-verbruik

**Tankboek**: houd per tankbeurt bij hoeveel liter je tankt, hoeveel km je gereden hebt en (optioneel) de literprijs.

Open `index.html` in je browser. Je ziet dan:

- bovenaan het formulier voor een nieuwe tankbeurt, met snelkeuzeknoppen voor je tankstation (Makro Duiven staat er altijd, daarna je meest gebruikte stations) en de literprijs van de vorige keer bij dat station
- verbruik per tankbeurt in L/100 km en "1 op X"
- gemiddeld verbruik, laatste tankbeurt en het gemiddelde van de laatste 5
- een grafiek met het lopend gemiddelde (je "equity curve") voor verbruik, literprijs of kosten per 100 km
- kosten per 100 km en totaal uitgegeven als je literprijzen invult

- een oliecheck: het Tankboek telt de kilometers van je tankbeurten en waarschuwt als het tijd is om het oliepeil te controleren (standaard na 1.500 km, zelf aan te passen)
- olie verversen: houdt de laatste verversing bij en waarschuwt na een instelbaar aantal kilometers of maanden, wat het eerst komt (standaard 15.000 km of 12 maanden)
- vloeistoffen: koelvloeistof, remvloeistof en ruitensproeiervloeistof, elk met een eigen waarschuwing na een instelbaar aantal kilometers en/of maanden (een veld op 0 zet dat deel uit)
- tabblad **Reiskosten**: vul de kilometers in, of zoek de afstand op tussen twee plaatsen, en zie wat een enkele reis en een retour kosten, op basis van je eigen verbruik en literprijs. Bij het typen krijg je suggesties (bijvoorbeeld Amsterdam Centraal, Zuid of Sloterdijk); er wordt alleen in Europa gezocht. Het opzoeken gebruikt Photon (OpenStreetMap) en OSRM en werkt alleen in de losse versie op GitHub Pages
- gemaakt voor de telefoon: tabbladen onderaan binnen duimbereik, grote knoppen en velden, onderhoud dat inklapt en vanzelf opent als er iets moet, een logboek met de laatste 5 tankbeurten en een bevestiging na het opslaan

In deze losse versie worden je tankbeurten in je browser bewaard (localStorage).

## Synchroniseren met GitHub

Open je Tankboek op GitHub Pages en klap onderaan **Synchroniseren met GitHub** open.

1. Maak een lege, **privé** repository aan voor je gegevens, bijvoorbeeld `benzine-gegevens`.
2. Maak een fine-grained token met alleen toegang tot die repository en **Contents: Read and write**.
3. Vul de repository en de token in het Tankboek in.

Je tankbeurten staan dan in `data/tankbeurten.json` in die privé-repository en zijn op al je apparaten hetzelfde.

- De token blijft alleen in de browser staan waarin je hem plakt.
- Elke wijziging maakt een commit in de gegevens-repository. Wijzigen en verwijderen werken ook tussen apparaten.
- Gebruik geen openbare repository voor de gegevens: daar kan iedereen het bestand lezen.

## Versies

Het versienummer staat bovenaan de pagina, onder de naam van de auto. Zo zie je of GitHub Pages de nieuwste versie toont.

- **1.7** (30 okt 2026): suggesties bij Van en Naar, alleen zoeken in Europa, route meteen opzoeken na het kiezen
- **1.6** (30 okt 2026): versienummer op de pagina
- **1.5** (30 okt 2026): formulier bovenaan, snelkeuze tankstation, tabblad Reiskosten, telefoonvriendelijk
- **1.4** (17 okt 2026): vloeistoffen (koel-, rem- en ruitensproeiervloeistof)
- **1.3** (17 okt 2026): olie verversen
- **1.2** (17 okt 2026): oliecheck
- **1.1** (14 okt 2026): synchroniseren met GitHub
- **1.0** (14 okt 2026): eerste versie van het Tankboek
