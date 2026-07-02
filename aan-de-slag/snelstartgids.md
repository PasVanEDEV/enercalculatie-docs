---
title: "Snelstartgids: eerste dossier in EnerCalculatie"
description: "Doorloop de 12-stappen workflow van EnerCalculatie en maak binnen vijf minuten uw eerste volledige energiecalculatie en adviesrapport voor een klantdossier."
---

Volg deze gids om snel en foutloos een dossier op te stellen. EnerCalculatie begeleidt u stap voor stap via een overzichtelijke 12-stappen workflow.

---

## 1. Account & Inloggen

### Inloggen

Ga naar [app.enercalculatie.nl](https://app.enercalculatie.nl), vil uw e-mailadres en wachtwoord in en klik op **Inloggen**.

<Frame>
  ![Image](/images/image.png)
</Frame>

---

## 2. Het Dashboard

Na het inloggen ziet u uw dashboard. Hier vindt u een overzicht van al uw dossiers. Klik op **Dossier aanmaken** om direct een nieuw klantdossier te starten.

<Frame>
  ![Image](/images/image-1.png)
</Frame>

---

## 3. Stappenplan (De 12 Workflow Stappen)

Via het linker menu doorloopt u de 12 stappen van het dossier:

| Stap | Scherm | Doel |
| :-- | :-- | :-- |
| **1** | Pand & Klantdossier Registratie | Pandgegevens, dakkenmerken en meterkast-specificaties invoeren |
| **2** | Slimme Documenten Uitlezer & AI OCR | Energierekening uploaden en automatisch laten uitlezen |
| **3** | Verbruiksprofiel & Energievraag | Uitgelezen verbruiksgegevens en tarieven controleren/aanvullen |
| **4** | Legplan & Zonnepanelen Dimensionering | Interactief legplan opstellen op de luchtfoto |
| **5** | Thuisbatterij & Energieopslag Configurator | Thuisbatterij configureren (inclusief dynamische netsturing) |
| **6** | Warmtepomp Configurator | Type warmtepomp selecteren en ISDE-subsidie berekenen |
| **7** | Airco & Lucht-Lucht Warmtepomp | Binnen- en buitenunits configureren per ruimte |
| **8** | Laadpaal Configurator (EV) | Type laadpaal en Load Balancing specificeren |
| **9** | ROI & Financiële Rendementsprognose | Automatisch gegenereerde businesscase en grafieken inzien |
| **10** | Technische Schouw - Overzicht | Alleen-lezen samenvatting van alle schouwgegevens controleren |
| **11** | Concept Adviesrapport & Offerte | Begeleidende brief schrijven (AI) en PDF/link genereren |
| **12** | Werkvoorbereiding & Logistiek | Bill of Materials (BOM) en installatie-instructies bekijken |

---

### Stap 1 - Pand & Klantdossier Registratie

Klik op **Pandgegevens** in het linker menu.

- **Locatie Details:** Voer postcode en huisnummer in. Het systeem haalt gegevens direct op uit de BAG-registratie (bouwjaar, type pand).
- **Gebruiks- & Gebouwprofiel:** Geef het daktype, dakhelling, dakoppervlak, energielabel en het aantal bewoners op.
- **Logistiek & Bereikbaarheid:** Noteer parkeermogelijkheden en benodigd klimmaterieel (zoals RSS-valbeveiliging).
- **Groepenkast & Elektra:** Selecteer type aansluiting (1-fase / 3-fase), hoofdzekering (A) en geef aan of er ruimte is in de meterkast.
- **Wandconstructie & Kabeltrajecten:** Selecteer de wandconstructie en beschrijf de kabelroute van de omvormer naar de meterkast.
- **Foto's uploaden:** Voeg foto's toe van de voorgevel, het dak en de groepenkast.

<Frame>
  ![Image](/images/image-2.png)
</Frame>

> \[!TIP\] Vul alle velden zo volledig mogelijk in. Ontbrekende gegevens worden in het schouwoverzicht (Stap 10) als leeg weergegeven.

---

### Stap 2 - Slimme Documenten Uitlezer & AI OCR

Klik op **AI Scan & OCR** in het linker menu.

1. Sleep de energierekening van de klant (PDF of smartphone-foto) naar het uploadveld of klik op het gebied om een bestand te selecteren.
2. De AI-engine analyseert het document op de achtergrond en haalt binnen 15 seconden de verbruiksgegevens en tarieven op.
3. De geëxtraheerde data wordt automatisch ingevuld in Stap 3.

<Frame>
  ![Image](/images/image-3.png)
</Frame>

---

### Stap 3 - Verbruiksprofiel & Energievraag

Klik op **Energieprofiel** in het linker menu.

- **Stroomverbruik:** Controleer het jaarverbruik (kWh/jaar), het leveringstarief en het teruglevertarief dat door de AI is uitgelezen.
- **Gasverbruik:** Controleer het jaarverbruik gas (m³) en het gastarief.
- **Netprofiel:** Selecteer het netcongestiegebied en geef aan of er een slimme meter aanwezig is.

<Frame>
  ![Image](/images/image-4.png)
</Frame>

> \[!TIP\] Heeft de klant geen energierekening bij de hand? Gebruik de gemiddelde landelijke waarden: ca. 3.000 kWh stroom en ca. 1.500 m³ gas per jaar voor een gemiddeld gezin.

---

### Stap 4 - Legplan & Zonnepanelen Dimensionering

Klik op **Zonnepanelen** in het linker menu.

1. **Legplan opstellen:** Het systeem toont een luchtfoto van het pand. Klik op de dakvlakken om panelen te plaatsen en pas eventueel helling en oriëntatie aan.
2. **Configuratie:** Selecteer het paneeltype uit uw catalogus (of voer het vermogen handmatig in) en kies het type omvormer (string of micro-omvormers).
3. **Live Metrics:** Rechts in het scherm ziet u direct de live impact op de jaaropbrengst (kWh), de zelfconsumptieratio en het opgesteld vermogen (kWp).

<Frame>
  ![Image](/images/image-5.png)
</Frame>

---

### Stap 5 - Thuisbatterij & Energieopslag Configurator

Klik op **Thuisbatterij** in het linker menu en zet de toggle **Thuisbatterij advies inschakelen** aan.

- **Catalogus & Capaciteit:** Kies een batterij uit uw assortiment en selecteer de capaciteit (5, 10, 15 of 20 kWh).
- **Arbitrage & Sturing:** Vink _Batterijsturing via dynamisch energiecontract inschakelen_ aan als de klant tariefarbitrage wil toepassen.
- **Plaatsing:** Selecteer de wandconstructie (verplicht voor de schouw) en geef de omgevingstemperatuur en kabelroute op.

<Frame>
  ![Image](/images/image-6.png)
</Frame>

> \[!IMPORTANT\] Een thuisbatterij vereist een slimme meter (SMR5 of vergelijkbaar) voor een correcte laadsturing. Controleer dit vooraf bij de klant.

---

### Stap 6 - Warmtepomp Configurator

Klik op **Warmtepomp** in het linker menu en zet de toggle **Warmtepompadvies inschakelen** aan.

- **Type & Vermogen:** Kies tussen Hybride of All-Electric, vul het thermisch vermogen (kW) en de verwachte SCOP in.
- **Huidige situatie:** Voer de huidige verwarmingsbron, het type afgiftesysteem (bijv. vloerverwarming) en het isolatieniveau in.
- **Plaatsing & Kosten:** Specificeer de locatie van de buitenunit, boilerinhoud en voer de investering en installatiekosten in. De ISDE-subsidie wordt automatisch getoond.

<Frame>
  ![Image](/images/image-7.png)
</Frame>

---

### Stap 7 - Airco & Lucht-Lucht Warmtepomp Configurator

Klik op **Airco** in het linker menu en zet de toggle **Airco-advies inschakelen** aan.

- **Systeem:** Kies het type systeem (bijv. Single-split of Multi-split) en selecteer eventueel een merkvoorkeur.
- **Binnenunits:** Voeg met de knop **\+ Unit toevoegen** een binnenunit toe voor elke te verwarmen of koelen ruimte.
- **Kosten:** Vul de geschatte totale investering in (exclusief BTW).

<Frame>
  ![Image](/images/image-8.png)
</Frame>

---

### Stap 8 - Laadpaal Configurator (EV)

Klik op **Laadpalen** in het linker menu en zet de toggle **Laadpaal advies inschakelen** aan.

- **Specificaties:** Selecteer het installatietype (wandmontage of montagepaal) en het laadvermogen (bijv. 11 kW / 3-fase).
- **Load Balancing:** Vink _Dynamic Load Balancing (DLB)_ aan indien gewenst. Dit voorkomt dat de hoofdzekering overbelast raakt tijdens het laden.
- **Kosten:** Voer de geschatte investering in (inclusief installatie, excl. BTW).

_\[SCREENSHOT: Laadpaal configurator\]_

---

### Stap 9 - ROI & Financiële Rendementsprognose

Klik op **Rendement & ROI** in het linker menu. _Dit scherm is volledig automatisch berekend._

- **25-Jaar Grafiek:** Toont het verschil tussen "Niets doen" (stijgende stroomkosten) en "Verduurzaamd Netto Bespaard".
- **Financiële Kengetallen:** Toont de terugverdientijd, het rendement (IRR), de netto contante waarde (NPV) en de besparing in jaar 1.
- **Gedetailleerde Opbouw:** Onderin vindt u een specificatie van de netto investeringen, BTW-verrekeningen en subsidies per maatregel.

_\[SCREENSHOT: ROI & Financiële Rendementsprognose\]_

---

### Stap 10 - Technische Schouw - Overzicht

Klik op **Schouw Overzicht** in het linker menu.

Dit is een alleen-lezen samenvatting van alle technische gegevens die tijdens de opname (Stap 1 t/m 8) zijn ingevoerd.

- Bovenaan de pagina verschijnt een **groene statusbalk** als alle verplichte velden succesvol zijn ingevuld.
- Ontbreken er nog kritieke velden? Dan toont de statusbalk precies welke gegevens u nog moet aanvullen.

_\[SCREENSHOT: Technische Schouw - Overzicht\]_

---

### Stap 11 - Concept Adviesrapport & Offerte

Klik op **Adviesrapport** in het linker menu.

- **AI Samenvatting:** Klik op _Schrijf AI Samenvatting_ om de Gemini AI automatisch een gepersonaliseerde toelichtingsbrief te laten schrijven voor uw klant.
- **Rapport exporteren:**
  - **Deel Rapport:** Genereert een interactieve, online link die u via e-mail of WhatsApp naar de klant stuurt.
  - **Rapport Afdrukken / PDF:** Download het rapport als een liggend A4 PDF-bestand.

_\[SCREENSHOT: Concept Adviesrapport & Offerte\]_

---

### Stap 12 - Werkvoorbereiding & Logistiek

Klik op **Werkvoorbereiding** in het linker menu. _Dit scherm is volledig automatisch berekend._

Hier wordt de **Bill of Materials (BOM)** gegenereerd voor uw installateurs:

- **Materiaallijst:** Zonnepanelen (aantal en oriëntatie), type omvormer en geschatte kabellengtes, batterij-type, warmtepomp, airco-units en de benodigde laadpaal-onderdelen.
- **Meterkast & Logistiek:** Type benodigde aardlekautomaat en het benodigde klimmaterieel op basis van de pandkenmerken.

_\[SCREENSHOT: Werkvoorbereiding & Logistiek\]_