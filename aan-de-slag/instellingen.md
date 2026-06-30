---
title: "Instellingen beheren"
description: "Beheer uw bedrijfsprofiel, berekeningsaannames, productcatalogus, tarieven en team"
---

Via het menu-item **Instellingen** (het tandwiel-pictogram in de navigatie) beheert u de globale configuratie van uw organisatie. Wijzigingen die u hier opslaat, worden direct toegepast op alle nieuwe berekeningen en rapporten.

---

## 1. Bedrijfsprofiel
De gegevens in het bedrijfsprofiel verschijnen automatisch op alle adviesrapporten en offertes die u genereert:

*   **Bedrijfslogo:** Upload een transparante PNG of SVG (max 500 KB) voor een professionele uitstraling in het rapport.
*   **Bedrijfsgegevens:** Vul uw handelsnaam, KvK-nummer (8 cijfers) en BTW-nummer in.
*   **Contactgegevens:** Uw zakelijke telefoonnummer, e-mailadres en website.
*   **Disclaimer (Rapport-footer):** De wettelijke disclaimer onderaan elk rapport. Deze is standaard juridisch gedetui-seerd, pas deze alleen aan na juridisch overleg.
*   **Applicatie Footer Tekst:** De tekst die in de voettekst van de applicatie zelf verschijnt.

*[SCREENSHOT: Toon de kaart Bedrijfsprofiel volledig ingevuld]*

---

## 2. Berekeningsaannames
De berekeningsaannames worden gebruikt in alle ROI-projecties en terugverdientijdberekeningen. De standaardwaarden zijn gebaseerd op actuele marktgemiddelden.

| Aanname | Standaardwaarde | Toelichting |
| :--- | :--- | :--- |
| **Projectieduur** | 25 jaar | De periode waarover de ROI wordt berekend (levensduur zonnepanelen). |
| **Energie-inflatie per jaar** | 2,5 % / jr | Verwachte jaarlijkse stijging van de energieprijzen. |
| **Paneeldegradatie per jaar** | 0,5 % / jr | Jaarlijks vermogensverlies van de zonnepanelen door veroudering. |
| **Basis zelfconsumptie** | 30 % | Percentage van de opgewekte stroom dat direct wordt verbruikt (zonder batterij). |
| **BTW-terugvordering batterij** | 80 % | Percentage van de BTW op een thuisbatterij dat kan worden teruggevorderd. |
| **Drempel batterij-aanbeveling** | € 200 / jr | Minimale besparing waarbij het systeem een thuisbatterij adviseert. |
| **SEEH-subsidie laadpaal (RVO)** | € 300 | Standaardbedrag SEEH-subsidie voor een laadpaal. |

> [!CAUTION]
> Wijzig de berekeningsaannames alleen als u zeker bent van de impact. Afwijkende waarden leiden tot onrealistische ROI-prognoses.

---

## 3. Productdatabase (Catalogus)
In de Productdatabase beheert u uw eigen assortiment. Producten die u hier toevoegt zijn direct beschikbaar in de configuratoren van Stap 4 (Zonnepanelen) en Stap 5 (Thuisbatterij).

### Zonnepanelen toevoegen
1. Klik op het tabblad **Zonnepanelen**.
2. Klik op **+ Paneel toevoegen**.
3. Vul de details in: merknaam, modelnaam, vermogen (Wp), afmetingen en prijs.
4. Klik op **Opslaan**.

### Thuisbatterijen toevoegen
1. Klik op het tabblad **Thuisbatterijen**.
2. Klik op **+ Batterij toevoegen**.
3. Vul de details in: merknaam, modelnaam, capaciteit (kWh), vermogen (kW) en prijs.
4. Klik op **Opslaan**.

*[SCREENSHOT: Productdatabase met het tabblad Zonnepanelen actief]*

> [!TIP]
> De catalogus is een handigheid, geen verplichting. U kunt in de configuratoren ook altijd handmatig een vermogen en prijs invoeren.

---

## 4. Tarieven & Prijzen
De tarieven en installatieprijzen die u hier instelt worden gebruikt als standaardwaarden in alle ROI-berekeningen en offertes. U kunt ze per dossier altijd overschrijven.

### Standaard Energietarieven (2026)
*   **Stroomtarief:** € 0,32 / kWh
*   **Gastarief:** € 1,35 / m³
*   **Teruglevertarief:** € 0,06 / kWh
*   **Teruglevering penalty (terugleverkosten):** € 0,08 / kWh

### Standaard Installatieprijzen (excl. BTW)
*   **Prijs per zonnepaneel:** € 350 / paneel
*   **Omvormer:** € 1.100
*   **Montage & installatie:** € 1.500
*   **Batterij:** € 480 / kWh

*[SCREENSHOT: De kaart Tarieven & Prijzen]*

---

## 5. Team & Gebruikersbeheer
Via **Team & Gebruikersbeheer** nodigt u collega's uit om samen in uw EnerCalculatie-omgeving te werken.

### Collega uitnodigen
1. Voer het e-mailadres van de collega in.
2. Selecteer de Rol:
    *   **Beheerder:** Volledige toegang (inclusief Instellingen, Account & Privacy en Stripe-facturatie).
    *   **Adviseur:** Alleen toegang tot het bewerken en aanmaken van dossiers. Geen toegang tot instellingen.
3. Klik op **+ Uitnodiging versturen**. De collega ontvangt een e-mail met een activatielink.

*[SCREENSHOT: Team & Gebruikersbeheer]*
