---
layout: default
title: Beispiel 1 – Suche nach IIIF
nav_exclude: true
---

# Beispiel 1 – Suche nach IIIF

Wie komme ich an die Image-API?

## Videoanleitung
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/U2-imF2-jhU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Schritt-für-Schritt-Anleitung

Viele Museen bieten ihre Werke in den Online-Sammlungen auch als IIIF kompatible Abbildungen an.

![Suche 1](https://cdn.lesliepzimmermann.de/storytelling/suche-(1).jpg)

Ob die Institution ihre Werke über IIIF bereitstellt, erkennen wir meist am IIIF-Logo, das sich in der Regel in der Nähe der Abbildung befindet.

![Suche 2](https://cdn.lesliepzimmermann.de/storytelling/suche-(2).jpg)

Auf der Seite der Smithsonian Institution, die uns hier als Beispiel dient, befindet sich der IIIF-Button direkt unter dem Bild, rechts neben der Download-Funktion. Wenn wir nun auf den Button klicken, dann werden zwei Optionen angezeigt.
Klicken wir auf den Punkt “View manifest”, so können wir uns das Manifest anzeigen lassen.
Klicken wir auf den Punkt “View in Mirador Viewer”, so öffnet sich die Ansicht der Abbildung im [Mirador Viewer](https://projectmirador.org/).

![Suche 3](https://cdn.lesliepzimmermann.de/storytelling/suche-(3).jpg)

Für unsere Digital Story benötigen wir die json-Datei der Image-API, die sich im Manifest befindet. Daher klicken wir auf “View manifest”.

![Suche 4](https://cdn.lesliepzimmermann.de/storytelling/suche-(4).jpg)

Nachdem wir das Manifest geöffnet haben, suchen wir die Image-API. Die Image-API folgt der entsprechenden Spezifikation und sieht in der Regel wie folgt aus: ```./full/full/0/default.jpg``` (im Screenshot blau markiert).

![Suche 5](https://cdn.lesliepzimmermann.de/storytelling/suche-(6).jpg)

Auf diese Adresse klicken wir nun und gelangen zur Abbildung.

![Suche 6](https://cdn.lesliepzimmermann.de/storytelling/suche-(7).jpg)

Jetzt benötigen wir die info.json-Datei. Dafür ändern wir in der Adresszeile die Endung von ```.../full/full/0/default.jpg``` in ```.../info.json```.

![Suche 7](https://cdn.lesliepzimmermann.de/storytelling/suche-(8).jpg)

So gelangen wir zu der info.json-Datei des Image API, die wir für die Implementierung unserer Story in den Storiiies-Editor benötigen.

![Suche 8](https://cdn.lesliepzimmermann.de/storytelling/suche-(9).jpg)

---

<span class="fs-8">
[Zurück](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/umsetzung-der-story-teil-1/){: .btn .btn-outline .mr-2 } 
</span>
<span class="fs-8">
[Weiter](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/suche-2/){: .btn .btn-outline}
</span>