---
title: A04-1 Hygrisches Klima
toc: true
header:
  image: /assets/images/04-splash.jpg
  image_description: "Unübersichtlich beschriebene Universitätstafel"
  caption: "Foto: Wikimedia Commons / CC0"
---

Walter-Lieth-Diagramme sind trotzt aller Ungenauigkeit immer noch ein beliebtes Darstellungsformat für die hydroklimatologische Charakterisierung eines Ortes in Schulbüchern und Atlanten. Im Rahmen dieses Arbeitsblatts sollen Sie Klimadaten aufbereiten und das hygrische Klima mittels eines [Walter-Lieth-Diagramms](https://de.wikipedia.org/wiki/Klimadiagramm) und  einer Verdunstungsabschätzung nach Haude vergleichen und bewerten.


## Aufgabe 04-1-L1: Walter-Lieth-Diagramm

{% capture A04-1-L1 %}

Erstellen Sie bitte ein Walter-Lieth-Diagramm auf Basis der langjährigen mittleren monatlichen Lufttemperatur und der langjährigen mittleren monatlichen Niederschlagssumme für die DWD-Station Cölbe auf Basis des in dem [zur Verfügung gestellten Datensatzes](https://ilias.uni-marburg.de/ilias.php?ref_id=1880380&cmd=view&cmdClass=ilrepositorygui&cmdNode=tt&baseClass=ilrepositorygui) enthaltenen Zeitraums. Lücken in der zur Verfügung gestellten Zeitserie müssen Sie dabei nicht explizit berücksichtigen.

Interpretieren Sie mit maximal zwei Sätzen das Walter-Lieth-Diagramm.

Umfang: 1 Seite in Ihrer PDF-Datei.
{% endcapture %}

<div class="notice--success">
  <h4 class="no_toc">Aufgabenstellung 04-1-L1:</h4>
  {{ A04-1-L1 | markdownify }}
</div>

## Aufgabe 04-1-L2: Verdunstung nach Haude

{% capture A04-1-L2 %}

Berechnen Sie bitte die langjährige mittlere monatliche potentielle Evapotranspiration nach Haude für den in A04-1-L1 bereits aufbereiteten Datensatz (siehe [Memo unten](#memo-verdunstung-nach-haude). Erstellen Sie bitte anschließend ein Diagramm, dass die potentielle Evapotranspiration den langjährigen monatlichen Niederschlagssumme gegenüberstellt.

Interpretieren Sie mit maximal zwei sätzen das Diagramm auf Basis der berechneten Evapotranspiration.

Umfang: 1 Seite in Ihrer PDF-Datei.
{% endcapture %}

<div class="notice--success">
  <h4 class="no_toc">Aufgabenstellung 04-1-L2:</h4>
  {{ A04-1-L2 | markdownify }}
</div>


## Aufgabe 04-1-L3: Walter-Lieth oder Haude?

{% capture A04-1-L3 %}

Diskutieren Sie die beiden erstellten Diagramme im Vergleich mit maximal zwei Sätzen. Nennen und Begründen Sie anschließend jeweils einen kritischen Punkt in der jeweiligen Darstellungs- bzw. Berechnungsform mit insgesamt maximal vier Sätzen.

Umfang: 1 Seite in Ihrer PDF-Datei.
{% endcapture %}

<div class="notice--success">
  <h4 class="no_toc">Aufgabenstellung 04-1-L3:</h4>
  {{ A04-1-L3 | markdownify }}
</div>


## Memo: Verdunstung nach Haude

Die Berechnung der Verdunstung nach Hause basiert auf der Formel:
```
PET = k ∗ e ∗ (1 - F / 100) [mm/d]
```
mit PET als die potentielle Evapotranspiration, k als der Haude-Faktor (siehe Tabelle), e als der Sättigungsdampfdruck um 14:00 in hPa, F als die relative Luftfeuchte in Prozent.

Der Sättigungsdampfdruck e [hPa] kann nach der Magnus-Formel z. B. wie folgt berechnet werden:
e = 6,11 ∗ 10^(7,48 ∗ T / (237 + T)) [hPa]
mit T als in diesem Falle die maximale Lufttemperatur in Grad Celsius.
Im Rahmen dieser Aufgabe können Sie anstelle der Temperatur um 14:00 Uhr die mittlere maximale Lufttemperatur sowie anstelle der Luftfeuchte um 14:00 Uhr die mittlere Luftfeuchte verwenden.
Die Haude-Faktoren sind in der nachfolgenden Tabelle nach [Hupfer et al. (2006)](https://www.springer.com/de/book/9783322967497) dargestellt:

|Monat      | Haude-Faktor|
|-----------|------|
| Januar    | 0,20 |
| Februar   | 0,20 |
| März      | 0,21 |
| April     | 0,29 |
| Mai       | 0,29 |
| Juni      | 0,28 |
| Juli      | 0,26 |
| August    | 0,25 |
| September | 0,23 |
| Oktober   | 0,22 |
| November  | 0,20 |
| Dezember  | 0,20 |