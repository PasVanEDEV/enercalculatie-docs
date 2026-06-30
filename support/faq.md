---
title: Veelgestelde vragen (FAQ)
description: Directe antwoorden op veelvoorkomende calculatievragen en support issues
---

Hieronder vindt u de meest gestelde vragen, onderverdeeld in vragen over de berekeningen, het gebruik van de applicatie, en vragen die wij vaak van installateurs krijgen.

## Algemene Support

### Ik zie een gele balk boven in mijn scherm?
Wanneer u een gele balk ziet met "STAGING", bevindt u zich in de testomgeving. Deze omgeving wordt gebruikt om nieuwe functies te testen en bevat testdata. Gebruik de reguliere productielink zonder balk voor uw echte klantendossiers.

### Mijn wijzigingen lijken niet te worden opgeslagen?
EnerCalculatie slaat uw gegevens automatisch op terwijl u typt (debounce). Let op de tekst "Opgeslagen om HH:MM" rechtsboven in uw scherm. Ziet u deze tekst niet updaten? Controleer dan uw internetverbinding.

### Waarom valt mijn warmteverliesberekening hoger uit dan de oude cv-ketel groot was?
Een cv-ketel is historisch vaak zwaar overgedimensioneerd (bijv. 24 kW of 30 kW) om snel warm tapwater te kunnen leveren. Het werkelijke verwarmingsvermogen ligt vaak veel lager. EnerCalculatie splitst dit zuiver uit, zodat u geen onnodig grote en dure warmtepomp selecteert.

### Wat moet ik invoeren als de exacte spouwisolatie onbekend is?
Als er geen bouwtechnische tekeningen zijn, selecteert u in EnerCalculatie het bouwjaar van de woning. De software past dan automatisch de *forfaitaire waarden* toe conform de ISSO-richtlijnen. Dit zijn historisch veilige aannames voor die specifieke bouwperiode.

### Wat is het effect van vloerkoeling op het energielabel?
Vloerkoeling (topkoeling) verhoogt het comfort in de zomer en zorgt ervoor dat u direct voldoet aan de **TO-juli** regelgeving. In de BENG-berekening kost het actieve koelen een kleine hoeveelheid elektriciteit (BENG 2), maar dit weegt ruimschoots op tegen het wegvallen van het oververhittingsrisico.


## AI & Data-extractie uit Energierekeningen

### 1. Elk format van de jaarnota is anders. Hoe weet ik zeker dat de AI de data wel 100% correct uitleest?
De AI-parser is specifiek getraind op de lay-outs van alle Nederlandse leveranciers (Eneco, Vattenfall, Essent, Tibber, etc.). Voordat de calculatie start, toont de interface een overzichtelijke verificatiestap waarin de adviseur de geëxtraheerde data in één oogopslag controleert en indien nodig direct aanpast.

### 2. Veel klanten leveren onleesbare foto's of scheve scans aan in plaats van een digitale PDF. Werkt het dan ook?
Onze software maakt gebruik van geavanceerde OCR (Optical Character Recognition) met ingebouwde perspectief- en contrastcorrectie. Hierdoor worden ook scherpe smartphone-foto's van geprinte facturen nauwkeurig uitgelezen.

### 3. Wat gebeurt er als de klant een onvolledige energierekening (bijvoorbeeld alleen de eerste pagina) uploadt?
Het systeem herkent direct of de cruciale verbruiks- en terugleverdata ontbreken. De adviseur krijgt meteen een melding welke pagina's of gegevens ontbreken, zodat er geen foute berekeningen worden gemaakt.

### 4. Ondersteunt de AI ook complexe, zakelijke grootverbruikfacturen met gecontracteerd vermogen?
Ja. De parser maakt onderscheid tussen kleinverbruik-aansluitingen en zakelijke grootverbruiknota's (inclusief piekbelasting en transportkosten), zodat je zowel de particuliere als de zakelijke markt kunt bedienen.

### 5. Wat doet de software met een rekening van een splinternieuwe of kleine energieleverancier?
De LLM-technologie achter onze parser zoekt niet naar vaste posities op de pagina, maar begrijpt de *context* van begrippen zoals 'levering', 'teruglevering', 'dal' en 'normaal'. Hierdoor worden nieuwe leveranciers direct correct geïnterpreteerd.

### 6. Hoe gaat de AI om met accounts die een dubbele meter (normaal-/daltarief) of juist een enkele meter hebben?
Het systeem herkent de meterstructuur automatisch. Bij een dubbele meter worden de verbruiken netjes gesplitst over de juiste tariefgroepen om de latere batterij- en PV-simulatie loepzuiver uit te voeren.

### 7. Onze adviseurs willen het gasverbruik vaak negeren. Filtert de AI dit eruit?
Ja. Het gasverbruik wordt apart geïdentificeerd. Je kunt in de instellingen aangeven of je dit wilt negeren, óf juist wilt gebruiken om de besparing van een toekomstige warmtepomp door te rekenen.

### 8. Duurt het parsen van zo'n zwaar document niet erg lang als het druk is op het platform?
Nee, de cloud-infrastructuur schaalt elastisch mee. De gemiddelde doorlooptijd van een upload naar een volledig ingevuld dataveld is minder dan 20 seconden, ongeacht de drukte.

### 9. Wat als de AI een typefout maakt in het klantadres?
Elk geëxtraheerd veld is direct bewerkbaar. De adviseur behoudt de controle en kan eventuele schoonheidsfoutjes binnen een seconde handmatig corrigeren in de interface.

### 10. Werkt de AI-parser ook als de energierekening in het Engels of Duits is opgesteld voor expats?
Ja, de AI is meertalig en herkent de energetische context (zoals *consumption* of *Lieferung*) probleemloos, om deze vervolgens correct te mappen naar het Nederlandse calculatiemodel.

## Rekenengine & Marktcomplexiteit

### 11. De salderingsregeling wordt afgebouwd of aangepast. Hoe houdt de software hier rekening mee?
Onze deterministische rekenengine bevat de wettelijke afbouwstaffels. Wijzigen de plannen in Den Haag? Dan updaten wij de rekenregels centraal in de achtergrond, waardoor jouw offertes direct voldoen aan de nieuwste wetgeving.

### 12. De terugleverkosten verschillen enorm per leverancier en veranderen continu. Hoe blijft dit nauwkeurig?
Wij houden een live database bij van de terugleverkosten en vaste leveringskosten van alle actieve Nederlandse energieleveranciers. De software koppelt de geüploade leverancier automatisch aan de meest actuele tariefmatrix.

### 13. Neemt de software de specifieke netbeheerderskosten (capaciteitstarief) ook mee in de ROI?
Ja. Op basis van de ingevoerde postcode herkent de software de actieve netbeheerder (zoals Liander, Enexis of Stedin) en past de exacte, actuele vastrecht- en transporttarieven toe.

### 14. Hoe accuraat zijn de berekeningen omtrent de energiebelasting en btw?
De engine rekent met de officiële belastingschijven en overheidsheffingen van de Belastingdienst voor het huidige kalenderjaar, inclusief de vermindering energiebelasting.

### 15. Welke stroomprijs-stijging hanteert de software voor de toekomst? Dit is vaak nattevingerwerk.
Standaard rekenen we met conservatieve marktprognoses, maar de beheerder van de tenant kan dit groeipercentage in het dashboard zelf aanpassen aan de eigen verkoopfilosofie.

### 16. Wij gebruiken Solar Monkey of 2Solar voor onze legplannen. Waarom hebben we jullie rekenengine nodig?
Legplan-software blinkt uit in dakinmeting, maar schiet tekort in diepgaande financiële energie-analyses (zoals dynamic pricing en batterij-sturing). EnerCalculatie voedt jouw legplan met de juiste data óf gebruikt de output ervan voor een waterdicht financieel voorstel.

### 17. Houdt de engine rekening met de specifieke geografische instralingsdata in Nederland?
Ja, de software maakt gebruik van de officiële KNMI-klimaatdata en instralingsdiagrammen voor Nederland om de opbrengst per windrichting en hellingshoek nauwkeurig te bepalen.

### 18. Kan de rekenengine omgaan met meerdere dakvlakken (bijvoorbeeld oost-west opstellingen)?
Ja. Je kunt eenvoudig meerdere segmenten invoeren in de calculatie. De engine berekent de gecombineerde opbrengstcurve over de dag heen, wat cruciaal is voor een correct batterij-advies.

### 19. Wordt de degradatie van de zonnepanelen meegenomen in de 25-jarige opbrengstberekening?
Ja, de software hanteert een instelbare lineaire degradatiefactor (bijvoorbeeld 0,5% per jaar) zodat de getoonde opbrengst over 15 of 25 jaar realistisch blijft.

### 20. Voldoen de berekeningen aan de geldende Nederlandse normen voor energieprestatie?
De algoritmes zijn afgestemd op de algemeen geaccepteerde NEN-methodieken voor het berekenen van de energieprestatie van gebouwen, wat zorgt voor een hoge mate van technische autoriteit richting de eindklant.

## Thuisbatterij & Opslag Simulaties

### 21. Het dimensioneren van een thuisbatterij is vaak gokken. Hoe bepaalt EnerCalculatie de ideale capaciteit?
De engine berekent de *sweet spot* door de uur-tot-uur opwekking van de zonnepanelen te leggen over het uur-tot-uur verbruiksprofiel van de klant. Hierdoor zie je exact bij welke batterijcapaciteit (kWh) de hoogste circulariteit en kortste terugverdientijd wordt behaald.

### 22. Kunnen jullie dynamic pricing (handelen op de EPEX-spotmarkt) accuraat simuleren voor een batterij?
Ja. De software simuleert de laad- en ontlaadcycli op basis van de daadwerkelijke historische EPEX-uurprijzen van het afgelopen jaar, inclusief de inkoop- en verkoopspreads en energiebelastingen.

### 23. Wordt de degradatie en de garantieperiode van de thuisbatterij meegewogen?
Zeker. De businesscase houdt rekening met de maximale cycli of de garantieperiode van de fabrikant (bijvoorbeeld 10 jaar) en toont transparant wanneer de batterij zichzelf heeft terugverdiend binnen of buiten deze periode.

### 24. Houdt de software rekening met het rendementsverlies (round-trip efficiency) van de omvormer en batterij?
Ja, de engine hanteert een standaard instelbaar rendementsverlies (bijvoorbeeld 10% tot 15% verlies bij laden/ontladen) om te voorkomen dat de opbrengst te optimistisch wordt voorgesteld.

### 25. Kunnen we de software ook inzetten voor zakelijke 'peak shaving' projecten?
Ja, de software kan de reductie van piekbelastingen simuleren voor MKB-bedrijven met een grootverbruikaansluiting, waardoor je direct de besparing op de transportkosten kunt aantonen.

### 26. Hoe houdt de berekening rekening met de aanwezigheid van een slim Energie Management Systeem (EMS)?
De engine simuleert een 'slimme sturingsstrategie' (laden bij negatieve prijzen/overcapaciteit, ontladen tijdens piektarieven), wat de meerwaarde van een EMS direct inzichtelijk maakt in de offerte.

### 27. Kan het systeem omgaan met het verschil tussen een 1-fase en een 3-fase aansluiting bij de selectie van een batterij?
Ja, bij de technische controle geeft het systeem een waarschuwing als de geselecteerde batterij of omvormer niet past bij de geëxtraheerde of ingevoerde hoofdaansluiting.

### 28. In de winter is er amper zon om de batterij te laden. Is jullie simulatie niet te rooskleurig?
Omdat de engine met een 365-dagenprofiel rekent, is de winterdip volledig zichtbaar. De software laat eerlijk zien dat de batterij in december voornamelijk stand-by staat of enkel op dynamische nettarieven handelt, wat het vertrouwen van de klant vergroot.

### 29. Wordt het risico op netcongestie (het uitschakelen van de omvormer) meegerekend?
Dit kan niet per adres voorspeld worden, maar je kunt in de algemene marge-instellingen een veiligheidsfactor toepassen om de opbrengst met een bepaald percentage te corrigeren voor congestiegevoelige regio's.

### 30. Kunnen we lokale subsidies voor energie-opslag handmatig toevoegen aan de berekening?
Ja. Je kunt per calculatie of centraal in de database subsidiebedragen definiëren die direct in mindering worden gebracht op de initiële investering in het financiële overzicht.

## Workflow, CRM & Software Koppelingen

### 31. Moeten onze adviseurs de data uit EnerCalculatie handmatig overtypen in ons CRM?
Nee. Via onze webhooks en open API kun je EnerCalculatie naadloos koppelen met systemen zoals HubSpot, Pipedrive of 2Solar, zodat de calculatieresultaten direct naar de juiste klantkaart worden gepusht.

### 32. Kunnen we de lay-out van de gegenereerde offerte volledig aanpassen aan onze eigen huisstijl?
Ja. In het Growth-pakket kun je je eigen logo uploaden, huiskleuren instellen, lettertypen kiezen en de opbouw van de tekstblokken volledig personaliseren.

### 33. Werkt de software goed op een tablet of smartphone als onze adviseurs bij de klant aan tafel zitten?
De applicatie is 100% responsive ontwikkeld. Adviseurs kunnen tijdens het keukentafelgesprek op een iPad de energierekening uploaden en direct de resultaten live aan de klant tonen.

### 34. Zit er een limiet aan het aantal adviseurs dat tegelijkertijd in ons account kan werken?
Nee. Onze software ondersteunt multi-user omgevingen. Afhankelijk van het gekozen pakket kunnen meerdere adviseurs gelijktijdig onafhankelijke calculaties uitvoeren zonder dat data elkaar overlapt.

### 35. Wij gebruiken een verouderd ERP-systeem zonder API. Kunnen we dan wel gebruikmaken van jullie data?
Ja. Elke calculatie kan met één klik worden geëxporteerd als een gestructureerd CSV- of Excel-bestand, zodat je de data handmatig kunt importeren in elk legacy-systeem.

### 36. Kunnen we rollen en rechten toewijzen, zodat adviseurs de algemene prijsinstellingen niet kunnen wijzigen?
Ja. Er is een strikt onderscheid tussen de 'Admin'-rol (die prijzen, marges en producten beheert) en de 'Adviseur'-rol (die enkel calculaties uitvoert en offertes genereert).

### 37. Hoe houden we overzicht als een klant drie verschillende smaakjes (offerte-versies) wil zien?
Binnen een klantdossier in EnerCalculatie kun je met één klik een calculatie kopiëren naar een 'Versie B' of 'Versie C', waarin je snel de batterijgrootte of het aantal panelen aanpast zonder de basisdata opnieuw in te voeren.

### 38. Duurt het genereren van de uiteindelijke PDF-offerte erg lang?
Nee, de PDF-generatie-engine draait aan de server-side en levert binnen 5 tot 10 seconden na het afronden van de calculatie een downloadbare, strakke PDF op.

### 39. Kunnen we naast PDF-energierekeningen ook directe slimme meterdata (zoals P1-exports) inlezen?
Ja, het systeem ondersteunt naast PDF-nota's ook de import van gestandaardiseerde uiterst nauwkeurige CSV-bestanden van P1-poort uitlezers.

### 40. Wordt de klant automatisch gemaild zodra de offerte klaar is?
Dit kun je zelf instellen. Je kunt ervoor kiezen de offerte eerst handmatig te controleren en te downloaden, of het systeem te automatiseren zodat de offerte direct via een gekoppelde mailserver naar de klant wordt verzonden.

## Maatwerk vs. Automatisering

### 41. Verliezen we door deze automatisering niet het persoonlijke, menselijke aspect van ons advies?
Juist niet. Omdat je adviseur niet meer anderhalf uur achter een Excel-sheet zit te ploeteren om data over te typen, heeft hij meer tijd over voor een kwalitatief en persoonlijk adviesgesprek met de klant.

### 42. Elk project heeft unieke marges of kortingen. Kunnen we die nog wel handmatig aanpassen per project?
Ja. De centrale instellingen dienen als blauwdruk (default waarden), maar de adviseur kan per unieke calculatie handmatig kortingen, toeslagen en specifieke margepercentages overschrijven.

### 43. Wij verkopen vaak met 'all-in' pakketprijzen. Kan de software daar wel mee rekenen?
Ja. Je kunt in de productcatalogus zowel werken met stuksprijzen (prijs per paneel/omvormer) als met vaste setprijzen (bijv. "Pakket 10 panelen inclusief montage voor €4.500").

### 44. Hoe verwerkt de software specifieke installatie-toeslagen, zoals een moeilijke kabelroute of steigerbouw?
Je kunt een lijst met veelvoorkomende installatie-toeslagen aanmaken in de database. De adviseur vinkt deze tijdens het proces simpelweg aan om ze direct op te nemen in de kostprijsberekening.

### 45. Kunnen we de tekst in de offerte nog handmatig aanpassen voordat de PDF wordt gegenereerd?
Ja, voor de definitieve generatie is er een 'Review'-scherm met een rich-text editor waarin specifieke opmerkingen of klantspecifieke afspraken handmatig kunnen worden toegevoegd.

### 46. Wij verkopen uitsluitend specifieke A-merken (zoals Enphase of SolarEdge). Kunnen we die hard coderen?
Je richt de productcatalogus volledig zelf in. De software toont in de keuze-menu's uitsluitend de merken, types en vermogens die jij daadwerkelijk op voorraad hebt of verkoopt.

### 47. Kan de software een berekening maken voor een klant die al zonnepanelen heeft en *alleen* een batterij wil toevoegen?
Ja. Je kunt bij de invoer aangeven dat er sprake is van een 'Bestaande PV-installatie'. Je vult het huidige vermogen en de jaaropbrengst in, en de engine berekent de ROI van de nieuwe batterij op basis van die bestaande situatie.

### 48. Kunnen we meerdere opties (bijv. Optie 1: Alleen PV, Optie 2: PV + Batterij) naast elkaar in één offerte presenteren?
Ja, de software ondersteunt 'multi-optie' presentaties in de PDF, waardoor de eindklant in één oogopslag het verschil in investering en terugverdientijd tussen de scenario's ziet.

### 49. Hoe gaan jullie om met tijdelijke kortingsacties van fabrikanten?
Die kun je eenvoudig tijdelijk activeren in je centrale productcatalogus met een begin- en einddatum, waarna de rekenengine hier automatisch rekening mee houdt.

### 50. Is de software geschikt voor grote, complexe bedrijfspanden met meerdere aansluitingen?
De focus ligt op de residentiële markt en het MKB. Voor gigantische industriële projecten met meerdere transformatorstations is specialistische engineeringsoftware nodig, maar voor 95% van je dagelijkse leads is EnerCalculatie perfect dekkend.

## Kosten & ROI van EnerCalculatie

### 51. De markt is momenteel rustig. Waarom zouden we nu maandelijks geld uitgeven aan software?
Juist nu de markt concurrerend is, overleef je op efficiëntie. Als je concurrent 2 uur doet over een offerte en jij stuurt hem binnen 5 minuten, win jij de klant. Het Starter-pakket kost minder dan de prijs van één verloren werkuur per maand.

### 52. Waarom betalen we een vast maandbedrag in plaats van een prijs per bruikbare calculatie (pay-per-use)?
Een vast maandbedrag zorgt voor voorspelbare softwarekosten zonder verrassingen achteraf. Hierdoor stimuleer je je adviseurs ook om *elke* lead door de software te halen, wat de algehele conversie verhoogt.

### 53. Zitten we direct vast aan een onbuigzaam jaarcontract?
Nee. We bieden flexibele maandabonnementen die maandelijks opzegbaar zijn. Pas wanneer je overtuigd bent van de waarde, kun je overstappen op een jaarcontract om te profiteren van 20% korting.

### 54. Zijn er verborgen kosten, zoals extra betalen voor het aantal AI-uploads?
Nee, transparantie staat voorop. De AI-uploads zijn volledig inbegrepen binnen de limieten van het gekozen pakket. Er zijn geen onverwachte kosten achteraf.

### 55. Rekenen jullie hoge opstart- of implementatiekosten om ons account in te richten?
Voor onze vroege instappers (de eerste 7 klanten) rekenen we €0,- setup-kosten. We helpen je kosteloos bij de initiële inrichting van je eerste tarieven en catalogus.

### 56. Hoe snel verdient deze software zichzelf concreet terug?
Gemiddeld bespaart een adviseur 1,5 uur per offerte. Bij een bescheiden volume van 30 offertes per maand bespaar je 45 uur aan kostbare manuren. Tegen een gemiddeld intern uurtarief van €40,- levert dit direct €1.800,- aan besparing op.

### 57. Wat kost het als we halverwege het jaar extra adviseurs (gebruikers) willen toevoegen?
Je kunt flexibel up- of downgraden tussen de pakketten. De upgrade naar het Growth-pakket (tot 5 gebruikers) is met één klik geregeld en wordt pro rata verrekend.

### 58. Wat gebeurt er met onze prijs als jullie de software in de toekomst duurder maken?
Als Launch Partner behoud je via onze *grandfather clause* je initiële lage instaptarief voor de rest van de levensduur van je contract. Prijsverhogingen gelden alleen voor nieuwe klanten.

### 59. Kunnen we een korting krijgen als we direct voor meerdere jaren tekenen?
We focussen nu op het jaarabonnement met 20% korting. Dit geeft de maximale balans tussen een scherpe prijs en flexibiliteit voor jouw onderneming.

### 60. Moeten we extra betalen voor support, hulp of updates van het systeem?
Nee. Technische support via e-mail en chat, evenals alle functionele en wettelijke software-updates, zijn volledig inbegrepen in de vaste abonnementsprijs.

## Data Security, Privacy & AVG

### 61. Verkopen of gebruiken jullie de geüploade verbruiksdata van onze klanten voor eigen energiediensten?
Absoluut niet. Wij zijn een pure B2B SaaS-leverancier. Jouw data en de data van jouw klanten zijn 100% jouw eigendom. Wij zullen nooit data commercialiseren of delen met derden.

### 62. Is jullie cloud-infrastructuur wel voldoende beveiligd tegen hackers?
Onze software draait op enterprise-grade cloud-infrastructuur (Supabase/Railway) die voldoet aan de strengste internationale veiligheidsnormen en beschikt over ISO 27001 en SOC2 certificeringen.

### 63. Waar ter wereld wordt de data van onze klanten fysiek opgeslagen?
Alle data wordt strikt binnen de grenzen van de Europese Unie (AWS/Supabase datacenters in Frankfurt en Amsterdam) opgeslagen en verwerkt, volledig in lijn met de Europese privacywetgeving.

### 64. Hoe gaan jullie om met het 'recht op vergetelheid' als een consument eist dat zijn data wordt gewist?
In het dashboard zit een ingebouwde 'Verwijder Klant'-knop. Hiermee wist het systeem met één klik alle persoonsgegevens, geüploade PDF's en calculatieresultaten definitief uit de database.

### 65. Is er een getekende verwerkersovereenkomst beschikbaar voor onze privacy-officer?
Ja. Bij het activeren van de tenant accoteer je digitaal onze standaard AVG-verwerkersovereenkomst (DPA), die volledig is opgesteld volgens de Nederlandse privacy-standaarden.

### 66. Wordt de data tijdens het uploaden en verzenden wel versleuteld?
Ja, alle datatransporten verlopen via hoogwaardige TLS 1.3 encryptieverbindingen (HTTPS). Data in rust in onze databases is bovendien versleuteld met AES-256 encryptie.

### 67. Maken jullie back-ups van onze calculaties voor het geval er iets misgaat?
Ja, er worden elke 24 uur volautomatische, incrementele back-ups gemaakt met een retentieperiode van 30 dagen, zodat we bij calamiteiten data snel kunnen herstellen.

### 68. Kunnen onze medewerkers inloggen via Two-Factor Authentication (2FA) om diefstal van accounts te voorkomen?
Ja, het platform ondersteunt 2FA via authenticator-apps (zoals Google Authenticator of Microsoft Authenticator) om de toegang tot de klantedatabase maximaal te beveiligen.

### 69. Hebben medewerkers van EnerCalculatie onbeperkt inzage in onze klantinformatie en marges?
Nee. Toegang tot klantspecifieke tenants is intern hermetisch afgesloten. Alleen in het geval van een supportaanvraag kan een gecertificeerde ontwikkelaar tijdelijk toegang krijgen, wat volledig gelogd wordt in een onwijzigbare audit-trail.

### 70. Is jullie privacyverklaring getoetst aan de richtlijnen van de Autoriteit Persoonsgegevens (AP)?
Ja, ons privacybeleid is opgesteld door juridische experts en sluit naadloos aan bij de strengste handhavingsrichtlijnen van de AP.

## Onboarding & Adoptie

### 71. Mijn adviseurs zijn niet technisch met computers. Gaan zij dit wel begrijpen?
De software is gebouwd volgens de 'zero-training' filosofie. Er zijn geen complexe menu's. Als een adviseur een bestand kan slepen en op 'berekenen' kan klikken, kan hij met EnerCalculatie werken.

### 72. Moeten we uren aan handleidingen doorlezen om te snappen hoe het werkt?
Nee. In de app is elke stap voorzien van korte, interactieve tooltips en videotutorials van maximaal 60 seconden die de werking direct visueel uitleggen.

### 73. Wat als we er tijdens de 30 dagen proefperiode zelf niet uitkomen met het inrichten van de prijzen?
Je staat er niet alleen voor. Tijdens de proefperiode plannen we een kosteloze 1-op-1 onboarding call waarin we samen jouw prijslijst en offertetemplate live in de software zetten.

### 74. Sommige van onze senior adviseurs zwerweren bij hun eigen Excel-sheet. Hoe overtuig ik hen?
Laat hen één keer hun moeilijkste casus handmatig uitrekenen, en doe daarna exact dezelfde casus live in EnerCalculatie binnen 3 minuten. De enorme tijdwinst en het feit dat ze sneller hun verkoopbonussen behalen, neemt de weerstand direct weg.

### 75. Het kost ons te veel tijd om de software te testen naast onze drukke dagelijkse werkzaamheden.
Het opzetten van een test-tenant kost letterlijk 10 minuten. Je test de software niet 'naast' je werk, maar *tijdens* je werk op een live lead. Het levert je vanaf de allereerste upload direct tijdswinst op.

### 76. Kunnen we onze productlijst (panelen/batterijen) via een Excel-bestand in één keer importeren?
Ja. We hebben een eenvoudige CSV/Excel-importfunctie. Je uploadt je huidige prijslijst en de catalogus in EnerCalculatie is direct gevuld.

### 77. Is het whitelabelen van de software ingewikkeld en hebben we daar een developer voor nodig?
Nee. Het is een kwestie van je logo slepen in de beheeromgeving en via een visuele kleurenkiezer de kleuren van je bedrijf aanklikken. De software past de interface en PDF direct automatisch aan.

### 78. Bieden jullie een duidelijke API-documentatie aan voor onze eigen IT-partij?
Ja, voor het Growth- en Enterprise-pakket stellen we een volledig gedocumenteerde REST API (inclusief Swagger/OpenAPI specificaties) ter beschikking waarmee je IT-partner direct aan de slag kan.

### 79. Wat gebeurt er als we na 30 dagen besluiten dat het niks voor ons is?
Geen enkel probleem. De proefperiode is 100% vrijblijvend en stopt automatisch. Er worden geen creditcardgegevens vooraf gevraagd, dus er is nul financieel risico.

### 80. Moeten we onze huidige CRM-software stopzetten om EnerCalculatie te kunnen gebruiken?
Nee, EnerCalculatie draait harmonieus *naast* of *als add-on op* je huidige systemen. Je hoeft niks te migreren of stop te zetten; je voegt enkel een krachtige reken- en parsemotor toe aan je bestaande keten.

## Commerciële Impact & Offerte-conversie

### 81. Waarom zou een snelle offerte de conversie verhogen? Consumenten beslissen hier toch niet binnen 5 minuten over?
Consumenten beslissen niet sneller, maar de *gunfactor* en de *attentiewaarde* zijn het hoogst op het moment dat de klant de aanvraag doet. De installateur die als eerste een professionele, kloppende offerte aanlevert, claimt de poleposition en wint in 60% of de gevallen de deal.

### 82. Wordt de offerte voor de consument niet veel te technisch door al die uur-simulaties?
Nee, de engine vertaalt de complexe achtergronddata naar glasheldere, visuele grafieken en overzichtelijke euro-bedragen. De klant ziet exact wat hij wil zien: "Wat kost het nu, wat bespaar ik per jaar, en wanneer is het terugverdiend?".

### 83. Geven jullie een garantie dat onze conversie stijgt met jullie software?
We kunnen geen harde conversiepercentages garanderen omdat de uiteindelijke verkoopkracht van je adviseur aan de telefoon ook meespeelt. Wel garanderen we een drastische verkorting van je salescyclus, wat historisch gezien bij B2B SaaS in deze sector altijd leidt tot een hogere win-rate.

### 84. Helpt de software ons ook herinneren wanneer we een uitgebrachte offerte moeten opvolgen?
Ja. In het dashboard zie je in één oogopslag welke offertes de status 'Verzonden' hebben en hoelang ze al openstaan, zodat je team proactief en warm kan opvolgen.

### 85. Kunnen we met de software eenvoudig cross-selling toepassen, zoals het direct aanbieden van een laadpaal?
Ja. Je kunt optionele producten toevoegen aan de offerte die de klant met één klik kan selecteren, wat de gemiddelde orderwaarde per geconverteerde lead verhoogt.

### 86. Grote, landelijke installateurs hebben enorme eigen IT-systemen. Kunnen wij als mkb-er wel tegen hen opboksen met jullie tool?
Juist wel. EnerCalculatie democratiseert deze geavanceerde AI- en rekenkracht. Met onze software beschikt een compact installatiebedrijf over exact dezelfde (of snellere) pre-sales technologie als de marktleiders, tegen een fractie van de kosten.

### 87. Kan de eindklant de offerte direct digitaal ondertekenen voor akkoord via jullie platform?
Ja. De online weergave van de offerte bevat een veilige digitale handtekening-module waarmee de klant direct akkoord kan geven, wat de drempel tot kopen aanzienlijk verlaagt.

### 88. Ziet de online offerte er wel goed uit op de smartphone van de consument?
De online offerte-omgeving is mobiel-geoptimaliseerd. De klant bekijkt de grafieken, ROI en de voorwaarden net zo vloeiend op zijn telefoon als op een desktop.

### 89. Kunnen we in de financiële weergave ook de optie voor een Duurzaamheidslening tonen?
Ja. Je kunt instellen dat het systeem naast de directe investering ook een rekenvoorbeeld toont op basis van de landelijke Energiebespaarlening, inclusief de maandelijkse lasten en directe besparingen.

### 90. Kunnen we zien of en wanneer de klant onze offerte digitaal heeft geopend?
Ja, het systeem beschikt over live tracking. Zodra de klant de link naar zijn voorstel opent, krijgt de betreffende adviseur direct een melding (of update in het CRM), wat hét perfecte moment is voor een opvolgtelefoontje.

## Toekomstbestendigheid & Support

### 91. Wat gebeurt er met onze softwarelicentie als EnerCalculatie onverhoopt besluit te stoppen?
Wij bouwen aan een winstgevend, stabiel SaaS-bedrijf op de lange termijn. Mocht er in een extreem scenario sprake zijn van stopzetting, dan treedt onze continuïteitsregeling in werking: alle broncodes en databases worden overgedragen aan een onafhankelijke stichting (escrow), zodat de software voor onze actieve gebruikers operationeel blijft.

### 92. Welke uptime-garantie (SLA) bieden jullie voor de software? We kunnen het ons niet veroorloven dat het systeem platligt.
Wij hanteren een uptime target van 99,9% voor onze kern-applicatie. Omdat we gebruikmaken van gedistribueerde cloud-architecturen, is de beschikbaarheid redundant en stabiel, ook tijdens zware piekbelastingen.

### 93. Kunnen we specifieke features aanvragen als we functionaliteit missen in de software?
Ja, we werken nauw samen met onze vroege gebruikers. In het dashboard vind je een 'Feature Request' sectie waar je ideeën kunt indienen en kunt stemmen op updates van andere installateurs. Veelgevraagde functies bouwen we kosteloos in.

### 94. Vinden software-updates overdag plaats, waardoor we hinder kunnen ondervinden tijdens werktijd?
Nee. Alle grote functionele updates en database-onderhoud worden uitsluitend uitgevoerd tijdens onze vaste onderhoudsvensters tussen 02:00 en 05:00 uur 's nachts, zodat je verkoop overdag 100% onverstoord doorgaat.

### 95. Is er een telefonische helpdesk beschikbaar als we direct een storing hebben in het hoogseizoen?
Voor het Growth- en Enterprise-pakket bieden we prioriteits-support met een gegarandeerde responstijd binnen twee uur via WhatsApp en chat, zodat kritieke problemen direct worden opgelost.

### 96. Hoe snel worden nieuwe panelen of batterijtypen van fabrikanten toegevoegd aan de algemene database?
Onze centrale productdatabase wordt wekelijks gescreend en geüpdatet met de nieuwste datasheets van populaire merken. Mis je een specifiek type? Dan voegen we die op verzoek binnen 24 uur handmatig voor je toe.

### 97. Is de software ook geschikt als we in de toekomst willen uitbreiden naar de Belgische of Duitse markt?
Onze focus ligt nu primair op het winnen van de Nederlandse markt vanwege de unieke complexiteit (saldering/terugleverkosten). Internationale uitbreiding staat op de roadmap, maar we zorgen er eerst voor dat we de onbetwiste specialist in Nederland zijn.

### 98. Wat gebeurt er als de onderliggende AI-modellen (zoals OpenAI of Anthropic) een storing hebben? Stopt EnerCalculatie dan ook?
Nee. Onze architectuur is 'model-agnostisch' en redundant opgebouwd. Mocht OpenAI een wereldwijde storing hebben, dan schakelt onze parser binnen milliseconden automatisch over naar een back-up model van Anthropic of een open-source alternatief op onze eigen servers.

### 99. Wordt de softwareprijs jaarlijks gecorrigeerd op basis van de inflatie?
Lopende jaarlicenties staan gedurende de contractduur volledig vast. Bij verlenging hanteren we een transparante indexering conform de CBS-richtlijnen, zonder onverwachte prijsexplosies.

### 100. Wat is de visie van EnerCalculatie op de lange termijn als de energiemarkt volledig omslaat naar Smart Grids?
Wij evolueren mee met de markt. EnerCalculatie wordt doorontwikkeld van een pre-sales rekentool naar een volwaardig energie-simulatieplatform dat klaar is voor Virtual Power Plants (VPP), Vehicle-to-Grid (V2G) en automatische netbalancering, zodat jouw software-investering ook over 5 of 10 jaar nog de standaard is.
