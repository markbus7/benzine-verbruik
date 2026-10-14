# benzine-verbruik

**Tankboek**: houd per tankbeurt bij hoeveel liter je tankt, hoeveel km je gereden hebt en (optioneel) de literprijs.

Open `index.html` in je browser. Je ziet dan:

- verbruik per tankbeurt in L/100 km en "1 op X"
- gemiddeld verbruik, laatste tankbeurt en het gemiddelde van de laatste 5
- een grafiek met het lopend gemiddelde (je "equity curve") voor verbruik, literprijs of kosten per 100 km
- kosten per 100 km en totaal uitgegeven als je literprijzen invult

In deze losse versie worden je tankbeurten in je browser bewaard (localStorage).

## Synchroniseren met GitHub

Open je Tankboek op GitHub Pages en klap onderaan **Synchroniseren met GitHub** open. Plak daar een fine-grained token met alleen toegang tot deze repository en **Contents: Read and write**. Je tankbeurten staan dan in `data/tankbeurten.json` en zijn op al je apparaten hetzelfde.

- De token blijft alleen in de browser staan waarin je hem plakt.
- Bij elke wijziging komt er een commit op `main`. Wijzigen en verwijderen werken ook tussen apparaten.
- Is de repository openbaar, dan is `data/tankbeurten.json` voor iedereen leesbaar.
