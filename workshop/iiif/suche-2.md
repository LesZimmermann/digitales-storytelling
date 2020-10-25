---
layout: default
title: Beispiel 2 – Suche nach IIIF
nav_exclude: true
---
# Beispiel 2 – Suche nach IIIF
Im folgenden Beispiel suchen wir die Image-API einer einzelnen Abbildung aus einem Werk, das mehrere Abbildungen enthält – in diesem Fall die als Buch publizierte [Leichenpredigt des Frankfurter Patriziers Johann Georg von Holzhausen](https://digital.staatsbibliothek-berlin.de/werkansicht/?PPN=PPN654654484).

Auf der Seite der Staatsbibliothek zu Berlin wird war kein IIIF-Logo angezeigt, doch die Staatsbibliothek stellt ihre Sammlung dennoch mittels IIIF zur Verfügung!

## Videoanleitung
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/GXIWdzuAioA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Schritt-für-Schritt-Anleitung

![Suche 1](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-01.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-01.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Um in diesem Fall an die Image-API zu kommen, klicken wir zunächst auf das Info-Kästchen links oben.

![Suche 2](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-02.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-02.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Nachdem wir etwas herunterscrollen, öffnen wir die Publikation durch den Klick auf [“Band im Mirador-Viewer öffnen”](https://mirador.staatsbibliothek-berlin.de/?manifest=https://content.staatsbibliothek-berlin.de/dc/654654484/manifest).

![Suche 3](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-03.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-03.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Da es sich bei dem Digitalisat der Publikation um ein mehrseitiges Werk handelt, müssen wir im Mirador-Viewer nun die gewünschte Seite mit der benötigten Abbildung suchen. Bei diesem Beispiel benötigen wir die Seite 5 mit dem Schabkunst-Bildnis des Johann Georg von Holzhausen. Wir klicken also auf das Icon der Seite 5.

![Suche 4](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-04.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-04.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Um an die für den Storiiies-Editor benötigte info.json-Datei der Abbildung zu kommen, öffnen wir nun einen neuen Tab. Mit Drag & Drop ziehen wir das kleine Icon der Seite 5 in die Adresszeile des Webbrowsers eines neuen Tabs.

![Suche 5](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-05.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-05.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Analog zum [Beispiel 1](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/suche-1/) löschen wir am Ende der Adresszeile ```full/51,/0/default.jpg``` und  ändern dieses in ```info.json```. Die URL sollten nun wie folgt aussehen: ```https://content.staatsbibliothek-berlin.de/dc/654654484-0005/info.json```

![Suche 6](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-06.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-06.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Die somit gewonnene URL können wir im nächsten Schritt zum Implementieren unserer Story in den Storiiies-Editor nutzen.

![Suche 7](https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-07.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/suche/suche-07.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

__Achtung:__ Nur im Firefox-Browser wird der json-Code lesbar dargestellt. Im Chrome-Browser braucht man ein Plugin oder man stellt den Code mit Websites wie https://jsonformatter.org/ dar.

---

<span class="fs-8">
[Zurück](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/suche-1/){: .btn .btn-outline .mr-2 } 
</span>
<span class="fs-8">
[Weiter](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/umsetzung-der-story-teil-2/){: .btn .btn-outline}
</span>