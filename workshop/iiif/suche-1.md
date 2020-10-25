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

![Suche 1](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-1.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-1.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Ob die Institution ihre Werke über IIIF bereitstellt, erkennen wir meist am IIIF-Logo, das sich in der Regel in der Nähe der Abbildung befindet.

![Suche 2](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-2.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-2.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Auf der Seite der Smithsonian Institution, die uns hier als Beispiel dient, befindet sich der IIIF-Button direkt unter dem Bild, rechts neben der Download-Funktion. Wenn wir nun auf den Button klicken, dann werden zwei Optionen angezeigt.
Klicken wir auf den Punkt “View manifest”, so können wir uns das Manifest anzeigen lassen.
Klicken wir auf den Punkt “View in Mirador Viewer”, so öffnet sich die Ansicht der Abbildung im [Mirador Viewer](https://projectmirador.org/).

![Suche 3](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-3.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-3.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Für unsere Digital Story benötigen wir die json-Datei der Image-API, die sich im Manifest befindet. Daher klicken wir auf “View manifest”.

![Suche 4](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-4.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-4.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Nachdem wir das Manifest geöffnet haben, suchen wir die Image-API. Die Image-API folgt der entsprechenden Spezifikation und sieht in der Regel wie folgt aus: ```./full/full/0/default.jpg``` (im Screenshot blau markiert).

![Suche 5](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-5.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-5.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Auf diese Adresse klicken wir nun und gelangen zur Abbildung.

![Suche 6](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-6.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-6.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Jetzt benötigen wir die info.json-Datei. Dafür ändern wir in der Adresszeile die Endung von ```.../full/full/0/default.jpg``` in ```.../info.json```.

![Suche 7](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-7.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-7.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

So gelangen wir zu der info.json-Datei des Image API, die wir für die Implementierung unserer Story in den Storiiies-Editor benötigen.

![Suche 8](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-8.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-8.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

---

<span class="fs-8">
[Zurück](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/umsetzung-der-story-teil-1/){: .btn .btn-outline .mr-2 } 
</span>
<span class="fs-8">
[Weiter](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/suche-2/){: .btn .btn-outline}
</span>