---
layout: default
title: 3.2 Umsetzung - Teil 1
nav_order: 2
parent: 3. Technische Umsetzung
---
# 3.2 Umsetzung der Story – Teil 1
{: .no_toc }
In diesem Kapitel werden wir unsere Story aus dem Storyboard (siehe Kapitel 2.4) mit dem Storiiies-Editor in die finale Form der Digitalen Story überführen. Der Storiiies-Editor ist ein einfaches und kostenloses Programm. Es bettet die einzelnen Annotationen, das heißt unsere im Storyboard zusammengestellten Textsegmente und Bildausschnitte, in ein ansprechendes Layout ein. Da Storiiies auf Websites eingebunden ist, kann der Inhalt anschließend mit der Community geteilt werden. Dabei arbeitet der Editor mit IIIF (siehe Kapitel 3.1), was es uns ermöglicht, hochauflösende Abbildungen zu verwenden, die wir direkt von den Online-Sammlungen mit der IIIF Image-API in Storiiies “verlinken” können. Wir haben aber auch die Möglichkeit, unsere eigenen Abbildungen im Storiiies-Editor hochzuladen. Beide Wege werden wir in diesem Kapitel beschreiben.

Hinweis: Da sich der Storiiies-Editor noch in der Entwicklung befindet und stetig verbessert wird, kann es sein, dass die Informationen aus diesem Kapitel stellenweise nicht mehr aktuell sind. Wir sind bemüht, den Workshop immer auf dem aktuellsten Stand zu halten. Wenn Dir/Ihnen dennoch Unstimmigkeiten auffallen, können diese gerne über unser [Feedback-Formular](https://leszimmermann.github.io/digitales-storytelling/feedback/) gemeldet werden!

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
__Autor:in__: Hier tragen wir unseren eigenen Namen ein.  
__E-Mail__: An dieser Stelle tragen wir unsere E-Mail-Adresse ein. Nach dem Erstellen der Story werden uns an diese Mailadresse die Links zu unserer Digitalen Story gesendet.    
__Beschreibung__:  Hier können wir eine kurze Beschreibung des Werkes oder der Story  einfügen.  
__Bildrechte__: Wichtig ist es an dieser Stelle zu vermerken, wem das Bild und die Bildrechte gehören.  

![Storiiies 1](https://cdn.lesliepzimmermann.de/storytelling/3-4/1_Diadem_Storiiies.jpg)

Hier sehen wir ein Beispiel für eine ausgefüllte Startseite:

![Storiiies 2](https://cdn.lesliepzimmermann.de/storytelling/3-4/2_Diadem_Storiiies.jpg)

### Bildhosting mit IIIF
Wollen wir die Bilddatei einer Online-Sammlung nutzen, die uns bereits ein Manifest oder einen Link zur info.json-Datei der Image-API anbietet, so können wir diese in die dafür vorgesehene Zeile des Editors kopieren.
Die Wege, um an Manifeste und Image-APIs (URLs; enden mit “info.json”) zu gelangen, sind nicht einheitlich. Unter Umständen können sich diese Wege ein wenig technisch gestalten.  Für technisch Interessierte stellen wir hier zwei Beispiele vor: [“Suche nach IIIF - Beispiel 1”](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/suche-1/) und [“Suche nach IIIF - Beispiel 2”](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/suche-2/). Unten finden sich bereits [copy-and-paste-fertige Beispiele](#beispiel) von info.json-Links der Image-APIs. Diese Links können einfach in Storiiies kopiert werden.

![Bildhosting mit IIIF](https://cdn.lesliepzimmermann.de/storytelling/Screenshot_04.jpg)

Einen ersten Anhaltspunkt, wie wir an IIIF-kompatible Abbildungen gelangen können, liefert das IIIF-Logo, welches sich meist in der Nähe der Abbildung in der Online-Sammlung befindet (siehe Abbildung). Dadurch gelangen wir an das Manifest oder die Image-API (URL), die wir in unseren Storiiies Editor kopieren können; wir müssen also keine Abbildungen downloaden. Mit dieser Methode können wir mit geringem Aufwand Digital Stories mit hochauflösenden Abbildungen erstellen, ohne viel Speicherplatz für große Bilddateien bereitstellen zu müssen. Eine Liste mit Datenbanken, in denen wir IIIF-APIs finden, haben wir unten zusammengestellt.

![Bildhosting mit IIIF - Getty](https://cdn.lesliepzimmermann.de/storytelling/2-2-1_Getty-2.jpg)
<p style="font-size: 0.8em;margin-top:-15px;">Das IIIF-Logo weist auf die IIIF-Kompatibilität hin.</p>

### Beispiel
Nun könnten wir das Manifest oder die Image-API für ein Bild unserer Wahl recherchieren. Für einen Schnellstart ohne Recherchearbeit stellen wir hier einige Beispiele bereit, die wir direkt in Storiiies einfügen können:  

Beispiel für Manifest:
[https://data.getty.edu/museum/api/iiif/130326/manifest.json](https://data.getty.edu/museum/api/iiif/130326/manifest.json)

Beispiel für Image-API:
[https://data.getty.edu/museum/api/iiif/18491/info.json](https://data.getty.edu/museum/api/iiif/18491/info.json)

### Bildhosting über Storiiies
Nutzen wir die Option, unser Bild über den Storiiies-Editor selbst zu hosten, wählen wir unter “Durchsuchen” eine jpg-Bilddatei auf unserem Computer aus und klicken anschließend auf “Upload”.

![Storiiies 3](https://cdn.lesliepzimmermann.de/storytelling/3-4/3_Diadem_Storiiies.jpg)

Wichtig: Bevor wir ein Bild hochladen, sollten wir uns sicher sein, dass wir über die Berechtigung dazu verfügen. Das Bild ist also entweder Open Source oder gehört uns selbst. Ist die Verwendung einer fremden Bilddatei rechtlich nicht erlaubt, so können wir sie auch nicht für eine Digitale Story verwenden.

Die Terms and Conditions finden wir auf der Startseite zum Erstellen einer Digitalen Story.

![Storiiies 5](https://cdn.lesliepzimmermann.de/storytelling/3-4/5_Diadem_Storiiies.jpg)

Haben wir die Bilddatei geladen sowie die Angaben zu Titel, Autor:in, unsere E-Mail-Adresse, die Beschreibung und die Hinweise zu den Bildrechten ausgefüllt, so können wir nun mit dem Storybuilding beginnen. Hierzu müssen wir den oben aufgeführten Nutzungsbestimmungen von Storiiies zustimmen und können anschließend nach dem Klick auf “Edit” mit dem Implementieren unseres Storyboards [Kapitel 2.4] beginnen.

![Storiiies 6](https://cdn.lesliepzimmermann.de/storytelling/3-4/6_Diadem_Storiiies.jpg)

Nachdem wir die Titelseite ausgefüllt und über “Edit” bestätigt haben, erhalten wir parallel eine E-Mail mit zwei Links. Rufen wir den ersten Link auf, gelangen wir jederzeit zum Editierungs-Menü unserer Story und können sie auch nachträglich noch bearbeiten. Dieser Link ist nur für uns bestimmt, sollte also nicht an andere weitergegeben werden.
Der zweite Link führt uns zum Viewer, mit dem wir die finale Version unserer Digitalen Story aufrufen können. Diesen Link teilen wir im Anschluss mit allen, die die Story sehen sollen.

Nun können wir in Teil 2 der Umsetzung unserer Story mit dem Implementieren unserer Textsegmente aus dem Storyboard beginnen und dazu die passenden Bildausschnitte auswählen (Link zu 3.2 Teil 2).

## Hilfreiche Links und Ressourcen
- [Storiiies Website](https://storiiies.cogapp.com/)
- [Andy Cummings von Cogapp präsentiert Storiiies](https://youtu.be/u4GC9ULypls)

### Online Sammlungen mit IIIF
Diese Sammlungen bieten den Download von Werken sowie die Möglichkeit, die Werke über die IIIF API zu nutzen.
Die folgende Karte bietet einen guten [Überblick über Institutionen](https://www.google.com/maps/d/viewer?mid=1faJRKJpj2Vau__RDwt8af040x0GTVozp&ll) an, die ihre Sammlung über die IIIF APIs anbieten:

<iframe src="https://www.google.com/maps/d/embed?mid=1faJRKJpj2Vau__RDwt8af040x0GTVozp" width="640" height="480"></iframe>

- [Getty Museum, Los Angeles](http://www.getty.edu/art/collection/)
- [Belvedere, Wien](https://sammlung.belvedere.at/)
- [National Gallery, Washington](https://www.nga.gov/collection.html)
- [Yale Center for British Art, New Haven](https://britishart.yale.edu/collections/using-collections/online-)
- [Smithsonian, Washington](https://www.si.edu/learn-explore)
- [Europeana](https://www.europeana.eu/en/search?query=sv_dcterms_conformsTo%3A%2aiiif%2a&view=grid)

### Online Sammlungen mit Creative-Commons (ohne IIIF)
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
[Zurück](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/was-ist-iiif/){: .btn .btn-outline .mr-2 }
</span>
<span class="fs-8">
[Weiter](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/umsetzung-der-story-teil-2/){: .btn .btn-outline}
</span>