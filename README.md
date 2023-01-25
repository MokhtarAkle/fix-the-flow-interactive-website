# Interactie Coding the Curbs map

## Link: https://mokhtarakle.github.io/the-client-case/

## Inhoudsopgave

  * [Beschrijving](#beschrijving)
  * [Kenmerken](#kenmerken)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)
  
## User Story
Als gebruiker wil ik gegevens kunnen opzoeken en filteren, zodat ik makkelijker achter informatie kom.

## Beschrijving
De focus van deze sprint ligt op interactie en informatie architectuur van een website. Ik heb dus gewerkt aan een nieuwe interactie toevoegen boven de bestaande interacties. Om bovenstaande user story op te lossen heb ik de eerder aangemaakte zoekfunctie werkend gemaakt en heb ik verbeteringen toegevoegd aan het bestaande filter systeem.

De zoekfunctie neemt adressen, plaatsnamen, bedrijfnamen etc aan en weergeeft deze vervolgens op de kaart met een bijbehorende marker. De kaart zoomt uit naar een level waarin je de verschillende smartzones om de locatie kan zien waarna je hier naar toe kan navigeren. De filterfunctie heeft een nieuwe functie toegevoegd gekregen waarmee wordt aangegeven welk filter is toegepast als deze geactiveerd wordt.

![image](https://user-images.githubusercontent.com/45001009/214432383-2b59db2e-3601-4e45-ab63-4577a0feec55.png)

![image](https://user-images.githubusercontent.com/45001009/214432490-b2e65d3d-a77b-450d-9954-5e38bec6d527.png)

![image](https://user-images.githubusercontent.com/45001009/214441051-1019e84e-4413-43fd-b70e-127fb09008cc.png)

## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met JS gedaan en hoe? -->
De zoekfunctie is gemaakt door gebruik te maken van de Places API van google, specifiek de Place autocomplete functie. Deze functie en de rest van de zoekfunctie zijn in JS gemaakt. Het filter systeem is met gebruik van JS en CSS gemaakt.

### Zoekfunctie

De zoekfunctie maakt gebruik van een text input element in HTML dat vervolgens in JS wordt toegevoegd aan een variabele. Er kunnen veel verschillende opties meegegeven worden aan de autocomplete functie om deze te personaliseren naar wens. Ik heb wat basis opties gebruikt om de zoek te focussen op Nederland en om de data te specificeren die teruggegeven wordt als iemand gebruik maakt van de functie. De HTML input en opties worden in een variabele samengevoegd als een nieuw Autocomplete element.

![image](https://user-images.githubusercontent.com/45001009/214455023-d16d4bc6-01f0-4f5d-89fd-fdc8151b9337.png)

Er wordt verder een eventlistener toegevoegd aan de autocomplete resultaten zodat de functie kan uitgevoerd worden als iemand een resultaat selecteert. Er wordt gebruik gemaakt van de Places API om custom icons toe te voegen aan de verschillende resultaten. Verder worden de gebruikelijke functies gebruikt om de kaart te centreren en te zoomen op de geselecteerde plaats.

![image](https://user-images.githubusercontent.com/45001009/214456397-ede370c1-beed-4c70-906d-c08fa0ba15da.png)

## Filterfunctie aanvulling

Om duidelijk te maken dat er een filter toegepast is en welke dit is, is er een nieuwe functie toegevoegd aan de bestaande filterfunctie om kaarten te weergeven met het huidig toegepaste filter. Er zijn lege elementen toegevoegd in HTML voor elke filteroptie die standaard verstopt zijn. Deze elementen worden gevuld met de waarde van het geselecteerde filter als hierop gedrukt wordt. Deze elementen worden weer leeggemaakt als een ander filter wordt geselecteerd en opnieuw aangevuld met de huidige waarde.

![image](https://user-images.githubusercontent.com/45001009/214456349-d05637dc-66f0-43cc-91a3-f43a7c394be2.png)


## Bronnen

[Place Autocomplete API](https://developers.google.com/maps/documentation/javascript/place-autocomplete)

## Licentie

![GNU GPL V3](https://www.gnu.org/graphics/gplv3-127x51.png)

This work is licensed under [GNU GPLv3](./LICENSE).
