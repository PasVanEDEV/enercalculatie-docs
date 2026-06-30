---
title: "Laadpalen (EV-Laders)"
description: "Het verschil tussen AC/DC laden, fasen en slimme functionaliteiten"---

Met de groei van elektrische voertuigen (EV's) wordt ook de thuislaadpaal een standaard onderdeel van de energie-installatie van een woning. In het rapportagemodel van EnerCalculatie kunnen laadpalen worden meegenomen in de totale berekening.

## AC vs DC Laden

| Type | Laadvermogen | Laadtijd (bij een 60 kWh accu) | Typisch Gebruik |
|---|---|---|---|
| **AC Thuislader (Wisselstroom)** | 3,7 kW / 7,4 kW / 11 kW / 22 kW | 16u / 8u / 5,5u / 2,7u | Thuis, bij bedrijfspanden, straatparkeren |
| **DC Snellader (Gelijkstroom)** | 50 kW – 350 kW | 30 tot 60 minuten | Publiek, langs snelwegen |

De meeste EV's worden thuis geladen met wisselstroom (AC). De auto zelf heeft een ingebouwde omvormer die dit omzet naar de gelijkstroom (DC) die de batterij nodig heeft.

## Belangrijke Termen

| Term | Uitleg |
|---|---|
| **kW (Laadvermogen)** | Hoe snel de auto laadt. Dit wordt bepaald door de zwakste schakel: de laadpaal óf de ingebouwde lader van de auto. |
| **kWh (Energie)** | Hoeveel energie de accu in totaal kan opslaan (de 'tankinhoud'). |
| **1-fase / 3-fase** | Een 1-fase aansluiting kan maximaal 7,4 kW laden. Voor sneller laden (11 of 22 kW) is een 3-fase aansluiting (krachtstroom) in de meterkast nodig. Dit vereist bij oudere woningen vaak een verzwaring via de netbeheerder. |
| **OCPP** | Open Charge Point Protocol. Een open standaard voor communicatie met de laadpaal, noodzakelijk voor backend-beheer en slim laden. |
| **Smart Charging** | Het laadvermogen past zich slim aan. Bijvoorbeeld door maximaal te laden wanneer de zonnepanelen veel opwekken, of wanneer het uurtarief (bij een dynamisch contract) erg laag is. |
| **Load Balancing** | Zorgt ervoor dat de hoofdzekering niet doorslaat. Als in huis veel stroom wordt verbruikt (bijv. oven + inductiekookplaat), wordt het vermogen naar de laadpaal tijdelijk 'geknepen'. |
| **V2H (Vehicle to Home)** | Bidirectioneel laden: de auto levert stroom terug aan de woning. De accu van de auto fungeert hierbij als een gigantische thuisbatterij. |
| **V2G (Vehicle to Grid)** | De auto levert stroom terug aan het openbare elektriciteitsnet om dit te balanceren. |

## Advies bij Offertes
Bij het configureren van een laadpaal in EnerCalculatie, houd u in gedachten:
- Controleer altijd of de huisaansluiting (bijv. 1x35A of 3x25A) voldoende is voor de gewenste lader.
- Vraag naar het type auto: Sommige hybrides kunnen maximaal op 1-fase (3,7 kW) laden, waardoor een dure 3-fase lader overbodig is.
