# benzine-verbruik

**Tankboek**: houd per tankbeurt bij hoeveel liter je tankt, hoeveel km je gereden hebt en (optioneel) de literprijs.

Open `index.html` in je browser. Je ziet dan:

- verbruik per tankbeurt in L/100 km en "1 op X"
- gemiddeld verbruik, laatste tankbeurt en het gemiddelde van de laatste 5
- een grafiek met het lopend gemiddelde (je "equity curve") voor verbruik, literprijs of kosten per 100 km
- kosten per 100 km en totaal uitgegeven als je literprijzen invult

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
