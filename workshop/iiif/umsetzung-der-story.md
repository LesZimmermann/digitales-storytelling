---
layout: default
title: 3.2 Umsetzung der Story - Teil 1
nav_order: 2
parent: 3. Technische Umsetzung
---
# 3.4 Umsetzung der Story
{: .no_toc }
In diesem Kapitel werden wir unsere Story aus dem Storyboard (siehe Kapitel 2.4) mit dem Storiiies-Editor in die finale Form der Digitalen Story überführen. Der Storiiies-Editor ist ein einfaches und kostenloses Programm. Es bettet die einzelnen Annotationen, das heißt unsere im Storyboard zusammengestellten Textsegmente und Bildausschnitte, in ein ansprechendes Layout ein. Da Storiiies auf Websites eingebunden ist, kann der Inhalt anschließend mit der Community geteilt werden. Dabei arbeitet der Editor mit IIIF (siehe Kapitel 3.1), was es uns ermöglicht, hochauflösende Abbildungen zu verwenden, die wir direkt von den Online-Sammlungen mit der IIIF Image-API (siehe Beispiele 1 & 2) in Storiiies “verlinken” können. Wir haben aber auch die Möglichkeit, unsere eigenen Abbildungen im Storiiies-Editor hochzuladen. Beide Wege werden wir in diesem Kapitel beschreiben. 

Hinweis: Da sich der Storiiies-Editor noch in der Entwicklung befindet und stetig verbessert wird, kann es sein, dass die Informationen aus diesem Kapitel stellenweise nicht mehr aktuell sind. Wir sind bemüht, den Workshop immer auf dem aktuellsten Stand zu halten. Wenn Dir/Ihnen dennoch Unstimmigkeiten auffallen, können diese gerne über unser Feedback-Formular (LINK) eingereicht werden!

## Inhalt
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Lernziele
- In diesem Kapitel lernen wir, wie wir unsere Story mit dem Storiiies-Editor in ihre finale Form überführen.

---

## Startseite erstellen und Bildhosting

[Zum Storiiies Editor](https://storiiies-editor.cogapp.com/){: .btn .btn-outline .mr-2 }

Auf der Startseite geben wir zunächst einige (Meta-)Daten zu unserer Abbildung und Story ein. Dabei können wir auswählen, ob wir unsere Abbildung über Storiiies hochladen oder ob wir eine Image-API, die mit “__info.json__” am Ende kenntlich gemacht ist, oder das Manifest der Presentation-API nutzen wollen.

__Titel__: Dies kann zum Beispiel der Titel des Werkes sein oder eine kreative Überschrift für die Story.
__Autor*in__: Hier tragen wir unseren eigenen Namen ein.  
__E-Mail__: An dieser Stelle tragen wir unsere E-Mail-Adresse ein. Nach dem Erstellen der Story werden uns an diese Mailadresse die Links zu unserer Digitalen Story gesendet.
__Beschreibung__:  Hier können wir eine kurze Beschreibung des Werkes oder der Story  einfügen.
__Bildrechte__: Wichtig ist es an dieser Stelle zu vermerken, wem das Bild und die Bildrechte gehören.

![Storiiies 1](https://cdn.lesliepzimmermann.de/storytelling/3-4/1_Diadem_Storiiies.jpg)

Hier sehen wir ein Beispiel für eine ausgefüllte Startseite:

![Storiiies 2](https://cdn.lesliepzimmermann.de/storytelling/3-4/2_Diadem_Storiiies.jpg)

### Bildhosting mit IIIF
Wollen wir die Bilddatei einer Online-Sammlung nutzen, die uns bereits ein Manifest oder eine IIIF-API (nochmal Link zu 3.1?) anbietet, so können wir diese in die dafür vorgesehene Zeile des Editors kopieren.
Die Wege, um an Manifeste und Image-APIs (URLs; enden mit “info.json”) zu gelangen, sind nicht einheitlich. Problematik an die IIIF-Dateien zu kommen… Für technisch Interessierte... Deshalb stellen wir hier zwei Beispiele vor: “Suche nach IIIF” (LINK). Unten finden sich noch Beispiele...

![Bildhosting mit IIIF](https://cdn.lesliepzimmermann.de/storytelling/Screenshot_04.jpg)

Einen ersten Anhaltspunkt, um an IIIF-kompatible Abbildungen zu gelangen, stellt das IIIF Logo dar, welches sich meist in der Nähe der Abbildung in der Online-Sammlung befindet (siehe Abbildung). Dadurch gelangen wir an das Manifest oder die Image-API (URL), die wir in unseren Storiiies Editor kopieren können, wir müssen also keine Abbildungen downloaden. Mit dieser Methode können wir mit geringem Aufwand Digital Stories mit hochauflösenden Abbildungen erstellen, ohne viel Speicherplatz für große Bilddateien bereitstellen zu müssen. Eine Liste mit Datenbanken, in denen wir IIIF-APIs finden, haben wir unten zusammengestellt. 

![Bildhosting mit IIIF - Getty](https://cdn.lesliepzimmermann.de/storytelling/2-2-1_Getty-2.jpg)

### Beispiel
Nun könnten wir Manifest oder Image-API für ein Bild unserer Wahl recherchieren. Für einen Schnellstart ohne Recherchearbeit stellen wir hier einige Beispiele bereit, die wir direkt in Storiiies einfügen können:  

Beispiel für Manifest:
https://data.getty.edu/museum/api/iiif/130326/manifest.json 

Beispiel für Image-API:
https://data.getty.edu/museum/api/iiif/18491/info.json

### Bildhosting: Über Storiiies
Nutzen wir die Option, unser Bild über den Storiiies-Editor selbst zu hosten, dann wählen wir unter “Durchsuchen” eine jpg-Bilddatei auf unserem Computer aus und klicken anschließend auf “Upload”.

![Storiiies 3](https://cdn.lesliepzimmermann.de/storytelling/3-4/3_Diadem_Storiiies.jpg)

Wichtig: Bevor wir ein Bild hochladen, sollten wir uns sicher sein, dass wir über die Berechtigung dazu verfügen. Das Bild ist also entweder Open Source oder gehört uns selbst. Ist die Verwendung einer fremden Bilddatei rechtlich nicht erlaubt, so können wir sie auch nicht für eine Digitale Story verwenden.

Die Terms and Conditions finden wir auf der Startseite zum Erstellen einer Digitalen Story.

![Storiiies 5](https://cdn.lesliepzimmermann.de/storytelling/3-4/5_Diadem_Storiiies.jpg)

Haben wir die Bilddatei geladen sowie die Angaben zu Titel, Autor*in, unsere E-Mail-Adresse, die Beschreibung und die Hinweise zu den Bildrechten ausgefüllt, so können wir nun mit dem Storybuilding beginnen. Hierzu müssen wir den oben aufgeführten Nutzungsbestimmungen von Storiiies zustimmen und können anschließend nach dem Klick auf “Edit” mit dem Implementieren unseres Storyboards [Kapitel 2.4] beginnen.

![Storiiies 6](https://cdn.lesliepzimmermann.de/storytelling/3-4/6_Diadem_Storiiies.jpg)

Nachdem wir die Titelseite ausgefüllt und über “Edit” bestätigt haben, erhalten wir parallel eine E-Mail mit zwei Links. Rufen wir den ersten Link auf, gelangen wir jederzeit zum Editierungs-Menü unserer Story und können sie auch nachträglich noch bearbeiten. Dieser Link ist nur für uns, sollte also nicht an andere weitergegeben werden.
Der zweite Link führt uns zum Viewer, mit dem wir die finale Version unserer Digitalen Story aufrufen können. Diesen Link teilen wir im Anschluss mit allen, die die Story sehen sollen.

Nun können wir in Teil 2 der Umsetzung unserer Story mit dem Implementieren unserer Textsegmente aus dem Storyboard beginnen und dazu die passenden Bildausschnitte auswählen (Link zu 3.2 Teil 2).

## Hilfreiche Links und Ressourcen:
[Andy Cummings von Cogapp präsentiert Storiiies](https://youtu.be/u4GC9ULypls)

### Online Sammlungen mit IIIF:
Diese Sammlungen bieten den Download von Werken sowie die Möglichkeit, die Werke über die IIIF API zu nutzen.
Die folgende Karte bietet einen guten Überblick über Institutionen an, die ihre Sammlung über die IIIF APIs anbieten:

https://www.google.com/maps/d/viewer?mid=1faJRKJpj2Vau__RDwt8af040x0GTVozp&ll

- [Getty Museum, Los Angeles](http://www.getty.edu/art/collection/)
- V&A
- Belvedere
- [National Gallery Washington](https://www.nga.gov/collection.html)
- [Europeana](https://www.europeana.eu/en/search?query=sv_dcterms_conformsTo%3A%2aiiif%2a&view=grid)
- https://www.deutsche-digitale-bibliothek.de/ (IIIF ?)
- https://iiif.biblissima.fr/#services-iiif
- [Yale Center for British Art](https://britishart.yale.edu/collections/using-collections/online-)
- [Smithsonian](https://www.si.edu/learn-explore)

### Online Sammlungen mit Creative-Commons (ohne IIIF):
Diese Sammlungen bieten zwar keine Schnittstelle über IIIF an, wir können die Werke trotzdem herunterladen und benutzen.
- Städel Museum, Frankfurt
- Metropolitan Museum of Art, New York
- Rijskmuseum, Amsterdam
- Kunsthistorisches Museum, Wien
- Staatliche Museen zu Berlin
- Museo del Prado, Madrid
- Musée du Louvre, Paris
- Bayerische Staatsgemäldesammlungen, München
- Szépművészeti Múzeum, Budapest

---

<span class="fs-8">
[Zurück](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/suche-2/){: .btn .btn-outline .mr-2 } 
</span>
<span class="fs-8">
[Weiter](https://leszimmermann.github.io/digitales-storytelling/workshop/ausblick/){: .btn .btn-outline}
</span>