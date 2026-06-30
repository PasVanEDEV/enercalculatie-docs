---
title: "Bouwfysica en schilberekeningen"
description: "Uitleg van thermische schil, Rc-waarde, U-waarde en luchtdichtheid voor correcte invoer van de gebouwschil in warmteverlies- en isolatieberekeningen."
---

Voor een correcte calculatie moet de thermische kwaliteit van de gebouwschil nauwkeurig worden ingevoerd. Hieronder vindt u het relevante vakjargon en de definities.

### Thermische schil
De isolerende jas van het gebouw. Alles wat de geconditioneerde binnenruimte scheidt van de onverwarmde buitenomgeving of de grond (vloer, gevel, dak, ramen en deuren).

### R_c-waarde (m²·K/W)
De **Warmteweerstand** van een samengesteld constructieonderdeel (bijv. een spouwmuur inclusief isolatie en luchtspouw). 
- *Betekenis:* Hoe hoger de R_c-waarde, hoe beter de constructie isoleert en hoe minder warmte er verloren gaat.
- *Praktijk:* Nieuwbouw vereist momenteel hoge waarden (bijv. gevel R_c ≥ 4,7).

### U-waarde (W/m²·K)
De **Warmtedoorgangscoëfficiënt** van specifieke elementen, hoofdzakelijk gebruikt voor glas en kozijnen.
- *Betekenis:* De hoeveelheid warmte die per seconde door één vierkante meter stroomt bij een temperatuurverschil van 1 Kelvin tussen binnen en buiten. 
- *Let op:* Hoe **lager** de U-waarde, hoe beter de isolatie. (Bijv. HR++ glas heeft een U-waarde van ca. 1,1; oud enkel glas zit rond de 5,0).

### Koudebrug (ψ-waarde / Psi)
Een lokale onderbreking of verzwakking van de isolatielaag (bijv. een doorlopende betonvloer naar buiten of een metalen kozijnanker). Dit veroorzaakt lokaal extra warmteverlies en verhoogt het risico op condensatie en schimmel. EnerCalculatie neemt dit lineaire warmteverlies automatisch mee via de forfaitaire toeslag of specifieke invoer.