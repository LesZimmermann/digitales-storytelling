---
layout: default
title: 3.5 Umsetzung der Story
nav_order: 6
parent: 3. Technische Umsetzung
---
# 3.5 Umsetzung der Story
{: .no_toc }
In diesem Kapitel werden wir Schritt für Schritt unsere Story aus dem Storyboard (siehe Kapitel 2.4) mit dem Storiiies Editor in die finale Form der Digitalen Story überführen – wir implementieren also unsere Story. Der Storiiies Editor ist ein einfaches und kostenloses Programm, das die einzelnen Annotationen, d. h. die Textsegmente und Bildausschnitte, in ein ansprechendes Layout bettet, welches auf Websites eingebunden und mit der Community geteilt werden kann. Dabei arbeitet der Editor mit IIIF, was es uns ermöglicht mit sehr großen Abbildungen zu arbeiten, die wir direkt von den Online-Sammlungen mit der IIIF Image-API (siehe Kapitel 3.X) in Storiiies “verlinken” können. Wir haben aber auch die Möglichkeit unsere Abbildungen im Storiiies Editor hochzuladen. Beide Wege werden wir in diesem Kapitel beschrieben. 

Hinweis: Da sich der Storiiies Editor noch in der Entwicklung befindet, kann es vorkommen, dass die Informationen aus diesem Kapitel nicht mehr aktuell sind. Wir sind bemüht, den Workshop immer auf dem aktuellsten Stand zu halten. Sollte Dir dennoch Unstimmigkeiten auffallen, gibt uns gerne über das Feedback-Formular (LINK) Bescheid. 

## Inhalt
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Lehrziele
Was wir in diesem Kapitel lernen:
- In diesem Kapitel lernen wir, wie wir unsere Story mit dem Storiiies Editor in ihre finale Form überführen.

---

[Zum Storiiies Editor](https://storiiies-editor.cogapp.com/){: .btn .btn-outline .mr-2 }

Auf der Startseite geben wir zuerst einige (Meta-)Informationen zu unserer Abbildung und zu unserer Story. Dabei können wir auch auswählen, ob wir unsere Abbildung über Storiiies hochladen oder ob wir eine Image-API, die mit “info.json” am Ende kenntlich gemacht ist, nutzen.

__Titel__: Dies kann zum Beispiel der Titel des Werkes sein oder eine kreative Überschrift für die Story. 
__Autor*in__: Hier tragen wir unseren eigenen Namen ein.
__E-Mail__: An dieser Stelle tragen wir unsere Mailadresse ein. Nach dem Erstellen der Story werden uns zu dieser Mailadresse die Links zu unserer Digitalen Story gesandt.
__Beschreibung__: Hier können wir z. B. eine kurze Beschreibung des Werkes oder der Story  einfügen. 
__Bildrechte__: Hier tragen wir ein, wem das Bild und die Bildrechte gehören.

![Storiiies 1](https://cdn.lesliepzimmermann.de/storytelling/3-4/1_Diadem_Storiiies.jpg)

Hier sehen wir ein Beispiel für eine ausgefüllte Startseite:

![Storiiies 2](https://cdn.lesliepzimmermann.de/storytelling/3-4/2_Diadem_Storiiies.jpg)

Wichtig: Bevor wir ein Bild hochladen, sollten wir uns sicher sein, dass wir über die Berechtigung dazu verfügen. Das Bild ist also entweder Open Source oder gehört uns selbst. Ist das Verwenden einer fremden Bilddatei rechtlich nicht erlaubt, so können wir sie auch nicht für eine Digitale Story verwenden.

Nun benötigen wir unseren Image API-Link. 

Nutzen wir hierfür die Option, unser Bild über den Storiiies-Editor selbst zu hosten, dann wählen wir unter “Durchsuchen” eine jpg-Bilddatei von unserem Computer aus und klicken anschließend auf “Upload”.

![Storiiies 3](https://cdn.lesliepzimmermann.de/storytelling/3-4/3_Diadem_Storiiies.jpg)

Wollen wir die Bilddatei einer Online-Sammlung nutzen, die uns bereits eine IIIF-API bzw. ein Manifest anbietet, so können wir diese in die dafür vorgesehene Zeile des Editors kopieren.
Zur Frage, wo sich IIIF-APIs (diese endet mit “info.json”) und ganze Manifeste finden lassen, siehe die Beispiele “Suche nach IIIF”.
Ferner besteht die Möglichkeit, eigene Bilddateien über einen externen Server zu hosten. Siehe hierzu “Exkurs IIIF-Hosting”.

![Storiiies 4](https://cdn.lesliepzimmermann.de/storytelling/3-4/4_Diadem_Storiiies.jpg)

Die Terms and Conditions finden wir auf der Startseite zum Erstellen einer Digitalen Story.

![Storiiies 5](https://cdn.lesliepzimmermann.de/storytelling/3-4/5_Diadem_Storiiies.jpg)

Haben wir die Bilddatei geladen sowie die Angaben zu Titel, Autor*in, unsere Mailadresse, die Beschreibung und die Hinweise zu den Bildrechten ausgefüllt, so können wir nun mit dem Storybuilding beginnen. Hierzu müssen wir zunächst noch den oben aufgeführten Nutzungsbestimmungen von Storiiies zustimmen und können anschließend nach dem Klick auf “Edit” mit dem Implementieren unseres Storyboards [Kapitel 2.4] beginnen.

![Storiiies 6](https://cdn.lesliepzimmermann.de/storytelling/3-4/6_Diadem_Storiiies.jpg)

Nachdem wir die Titelseite ausgefüllt und über “Edit” bestätigt haben, erhalten wir parallel eine Mail mit zwei Links. Rufen wir den ersten Link auf, gelangen wir jederzeit zum Editierungs-Menü unserer Story und können sie auch nachträglich noch bearbeiten. Dieser Link ist nur für uns, sollte also nicht an andere weitergegeben werden.
Der zweite Link führt uns zum Viewer, mit dem wir unsere fertige Digitale Story aufrufen können. Diesen Link teilen wir im Anschluss mit allen, die die Story sehen sollen.

Das Implementieren unseres Storyboards in den Storiiies-Editor funktioniert schrittweise:

Oben links besteht mit dem Feld “Add new” die Möglichkeit einen Bildausschnitt, den wir auf der rechten Seite sehen, mit einer Textannotation zu versehen.

![Storiiies 7](https://cdn.lesliepzimmermann.de/storytelling/3-4/7_Diadem_Storiiies.jpg)

Nun können wir per copy and paste die Textannotationen aus dem Storyboard...

![Storiiies 8](https://cdn.lesliepzimmermann.de/storytelling/3-4/8_Diadem_Storiiies.jpg)

...in das Textfeld des Storiiies-Editors einfügen.

![Storiiies 9](https://cdn.lesliepzimmermann.de/storytelling/3-4/9_Diadem_Storiiies.jpg)

Nun müssen wir zur Annotation den entsprechenden Bildausschnitt auswählen, den wir im Storyboard festgelegt haben. Hierzu stehen auf der rechten Seite des Editors die Lupen-Werkzeuge zum Hinein- bzw. Herauszoomen bereit. Alternativ kann man den Bildausschnitt auch mit dem Mausrad verkleinern und vergrößern.

![Storiiies 10](https://cdn.lesliepzimmermann.de/storytelling/3-4/10_Diadem_Storiiies.jpg)

Sind wir mit dem Bildausschnitt zufrieden, können wir ihn zusammen mit der Textannotation durch das Klicken auf “Submit” bestätigen.

![Storiiies 11](https://cdn.lesliepzimmermann.de/storytelling/3-4/11_Diadem_Storiiies.jpg)

Soll eine Annotation noch einmal bearbeitet oder gar gelöscht oder der Bildausschnitt neu gewählt werden, findet sich dazu unter der Textbox die Optionen “Edit” zum Bearbeiten des Textes und des Bildausschnitts und “Delete” zum Löschen.

![Storiiies 12](https://cdn.lesliepzimmermann.de/storytelling/3-4/12_Diadem_Storiiies.jpg)

Anschließend wird die Änderung durch einen Klick auf “Update” übernommen.

![Storiiies 13](https://cdn.lesliepzimmermann.de/storytelling/3-4/13_Diadem_Storiiies.jpg)

Nun fügen wir Schritt für Schritt durch Klicken auf “Add new” all unsere Textsegmente aus dem Storyboard in den Editor und wählen den dazugehörigen Bildausschnitt.

![Storiiies 14](https://cdn.lesliepzimmermann.de/storytelling/3-4/14_Diadem_Storiiies.jpg)

Per drag and drop kann die Reihenfolge der Annotationen, falls gewünscht, immer wieder verändert werden. Die einzelnen Texte lassen sich nach wie vor zu jeder Zeit bearbeiten.

![Storiiies 15](https://cdn.lesliepzimmermann.de/storytelling/3-4/15_Diadem_Storiiies.jpg)

Über die Schaltfläche “Links” gelangen wir zu den zwei Links, die uns per Mail nach dem Ausfüllen der Titelseite gesendet worden sind. Der obere der beiden Links ist jener, der mit allen geteilt werden kann, die die fertige Story zu sehen bekommen sollen.
Mit dem unteren Link gelangt man jederzeit in den Editor, um etwas in der Story zu verbessern oder ändern. Wie schon gesagt: Dieser Link ist nur für uns selbst gedacht und sollte nicht mit anderen geteilt werden.
Zusätzlich findet sich unter den beiden Links noch ein Code, der zum Einbetten der Digitalen Story auf eine (eigene) Website gedacht ist.

![Storiiies 16](https://cdn.lesliepzimmermann.de/storytelling/3-4/16_Diadem_Storiiies.jpg)

Klicken wir auf “Preview”, so können wir eine Vorschau unserer Digitalen Story ansehen. 

![Storiiies 17](https://cdn.lesliepzimmermann.de/storytelling/3-4/17_Diadem_Storiiies.jpg)

Geschafft! Nun können wir uns unsere fertige Digitale Story ansehen.
Zur Erinnerung: Wir haben jederzeit die Möglichkeit, etwas an der Story zu ändern, sollten uns z. B. Rechtschreibfehler oder Zahlendreher etc. auffallen.

![Storiiies 18](https://cdn.lesliepzimmermann.de/storytelling/3-4/18_Diadem_Storiiies.jpg)

Über die Pfeile können wir innerhalb der Digitalen Story navigieren, vor- und zurück.

![Storiiies 19](https://cdn.lesliepzimmermann.de/storytelling/3-4/19_Diadem_Storiiies.jpg)

Beim Lesen der Story ist es uns stets möglich, auch an andere Stellen des Kunstwerkes zu zoomen oder sich an eine andere Stelle zu bewegen. Dazu nutzen wir einfach die Maus bzw. das Mausrad.

![Storiiies 20](https://cdn.lesliepzimmermann.de/storytelling/3-4/20_Diadem_Storiiies.jpg)

Über das Augensymbol links oben können wir die Textannotationen ein- und ausblenden.

![Storiiies 21](https://cdn.lesliepzimmermann.de/storytelling/3-4/21_Diadem_Storiiies.jpg)

Tipp: Es ist ratsam, sich auch schon nach dem Einfügen der ersten Textannotationen eine Vorschau der Story anzeigen zu lassen. Dies dient dazu, ein Gefühl für das Erscheinungsbild zu bekommen. Sind unsere Annotationen vielleicht zu lang? Muss man Scrollen, um sie ganz lesen zu können?
Des Weiteren ist es nützlich, sich die Story auch beispielsweise auf dem Smartphone anzusehen. Hier wird noch deutlicher, dass es auf den Umfang der Textannotationen ankommt. Pro Annotation sollte der Text so kurz wie möglich, aber so ausführlich wie nötig sein. Eine Alternative zum Wegkürzen wäre es, ein Textsegment auf zwei Annotationen aufzuteilen. Wir sollten dabei allerdings stets auch den Umfang der gesamten Digitalen Story nicht aus dem Blick verlieren. Um den Umfang zu überprüfen, können wir die Story vorab jemandem zum Lesen geben und uns Feedback einholen oder selbst die Zeit stoppen, die wir benötigen, um uns einmal durch die gesamte Story zu klicken.

![Storiiies 22](https://cdn.lesliepzimmermann.de/storytelling/3-4/22_Diadem_Storiiies.jpg)

<iframe width="100%" height="480" src="https://storiiies.cogapp.com/viewer/ea1dl/Diamonds-are-a-girls-best-friend-Das-DiamantDiadem-von-Marjorie-Merriweather-Post?embed=true" title="Diamonds are a girl's best friend - Das Diamant-Diadem von Marjorie Merriweather Post"></iframe>

---

[folgt...]

<span class="fs-8">
[Zurück](https://leszimmermann.github.io/digitales-storytelling/workshop/digitales-storytelling/eine-story-entwickeln/){: .btn .btn-outline .mr-2 } 
</span>
<span class="fs-8">
[Weiter](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/technische-umsetzung/){: .btn .btn-outline}
</span>