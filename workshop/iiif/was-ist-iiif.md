---
layout: default
title: 3.1 Was ist IIIF?
nav_order: 1
parent: 3. Technische Umsetzung
---
# 3.1 Was ist IIIF?
{: .no_toc }
Die Digitalisierung von Kulturgütern, etwa zum Zweck der Vermittlung oder Forschung, hat seit den 1990er Jahren stark zugenommen. Immer mehr Museen, Bibliotheken, Archive und Kultureinrichtungen haben seither ihre eigenen Bestände digitalisiert und diese ganz oder teilweise der Öffentlichkeit zur Verfügung gestellt. Doch gab es hierfür zunächst kein Standardvorgehen. In verschiedenen Institutionen wurden unterschiedliche Wege gewählt, sodass auch die unterschiedlichen digitalen Bildspeicher uneinheitlich sind. Forschende und Interessierte müssen sich also mit einer Vielzahl verschiedener Formate auseinandersetzen, wenn sie die digitalisierten Bilder nutzen wollen.

Um die Kompatibilität digitaler Daten zu verbessern, hat die IIIF Community mit ihrem Framework seit dem Jahr 2011 einen Lösungsvorschlag geliefert, der mittlerweile zu einem Standard avanciert ist und von zahlreichen Institutionen weltweit genutzt wird. Da IIIF in einem Open Source Framework läuft, entwickelt es sich aufgrund des Engagements der Community fortlaufend weiter.

Aus der Digitalisierung von Bibliotheks- und Archivbeständen kommend, erleichtert IIIF auch Kunsthistoriker:innen die Arbeit; der vielseitige Standard lässt sich für Forschungs- und Vermittlungszwecke ideal nutzen. Dies wird auch im nächsten Kapitel unseres Workshops deutlich; hier setzen wir IIIF ein, um eine Digitale Story zu erzählen. Dabei läuft IIIF mehr oder weniger im Hintergrund, das heißt unter Umständen bemerken wir gar nicht, dass wir mit diesem Programm arbeiten. Dennoch sind einige Grundkenntnisse zu IIIF sehr hilfreich: Geübte Nutzer:innen merken sofort, ob mit IIIF im Hintergrund gearbeitet wird, und können sich leicht einige Praktiken aneignen, die die Möglichkeiten in der Handhabung digitaler Bilder wesentlich erweitern.

## Inhalt
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Lernziele
 - In diesem Kapitel lernen wir etwas über den neuen Bildstandard IIIF, seinen Nutzen und Mehrwert gegenüber der herkömmlichen Verwendung von Bildmaterial.
- Kennenlernen des Storiiies-Editors von Cogapp

---

## Was ist IIIF?
Bei IIIF (“triple-eye-eff”) handelt es sich um eine Programmierschnittstelle. Die Nutzung von IIIF ist ein Übereinkommen von Institutionen, die ihr digitales Bildmaterial einheitlich zur Verfügung stellen, um die Kompatibilität der Bilder zu vereinfachen.

Der Vorteil für die Institutionen liegt darin, dass sie durch die Nutzung der Schnittstelle auf die große Infrastruktur, die um IIIF herum entwickelt worden ist und ständig weiterentwickelt wird, zugreifen können. Dadurch muss sich zum Beispiel nicht jede Bibliothek um die Programmierung eines eigenen Bild-Viewers kümmern. Denn alle Bilder, die mit der IIIF Schnittstelle kompatibel sind, können mit einem IIIF fähigen Viewer betrachtet werden, der als Open Source Software im WWW zur Verfügung steht.

Dies hat auch für uns als Nutzer*innen einige Vorteile. Wir können zum Beispiel im Viewer des Getty Museums in Los Angeles ein Bild in hoher Auflösung betrachten und gleichzeitig ein weiteres aus der National Gallery London einfügen. Die Bilder können nun nebeneinander detailliert betrachtet und verglichen werden, ohne dass diese heruntergeladen werden müssen.

[Video]

Auch der Storiiies-Editor, den wir zur Umsetzung unserer Story benutzen, basiert auf IIIF. Wie wir im folgenden Kapitel sehen werden, können wir einfach den Link zu einem IIIF-Bild einfügen und damit arbeiten, ohne dass wir ein Bild erst aus einer Online-Sammlung auf unseren Rechner herunterladen und dann in Storiiies hochladen müssen (diese Möglichkeit besteht allerdings bei Bedarf natürlich auch). Außerdem können wir dadurch mit hochauflösenden Abbildungen arbeiten:  Storiiies lädt immer die richtige Auflösung, je nachdem wie tief wir in das Bild hineingezoomt haben. Das Bild wird nämlich direkt vom Server der Institution geladen, wo es meist in deutlich höherer Auflösung liegt, als wir es selbst herunterladen könnten. IIIF Abbildungen werden dabei ähnlich aufgerufen wie eine Website, nämlich über eine URL (z.B. https://…). Diese Links können wir entweder direkt im Browser in die Adresszeile tippen oder etwa in einen Viewer oder Storiiies.

Generell sind zwei unterschiedliche Arten von IIIF Links (= Schnittstellen) zu unterscheiden. Zum einen gibt es einen Link, der uns direkt zum Bild führt, hier sprechen wir von Image-API (Bild-Programmierschnittstelle). Zum anderen gibt es einen Link, der Informationen über das Bild enthält, hier sprechen wir von Presentation-API (Präsentations-Programmierschnittstelle). Anstelle von Presentation-API ist oftmals auch von einem Manifest die Rede. Es enthält Metadaten und man kann es sich als eine Art Rezept für die Darstellung von Bildern vorstellen. Hier können neben dem Titel der Abbildung und der Bildgröße auch (unsere) Annotationen enthalten sein.

Die Image-API können wir über eine URL aufrufen und sogar steuern. Das heißt, dass wir durch die Eingabe von bestimmten Parametern die Darstellung der Abbildung anpassen können. So führt zum Beispiel die Änderung von ```https://ids.si.edu/ids/iiif/NMAH-ET2011-40071/full/full/0/default.jpg``` zu ```https://ids.si.edu/ids/iiif/NMAH-ET2011-40071/810,970,450,450/full/0/default.jpg``` dazu, dass nur ein Ausschnitt der Abbildung dargestellt wird. Im Grunde übernehmen wir dabei die Aufgabe eines Computerprogramms, das bei unserer Betrachtung und Steuerung über die Tasten des Viewers nichts anderes macht, als diese Befehle in die Adresszeile zu schreiben, die wir in diesem Fall nicht sehen würden.

Probieren wir das Ganze doch einmal aus:

1. Über den folgenden Link per Image-API ein Bild aufrufen: ```https://ids.si.edu/ids/iiif/NMAH-ET2011-40071/full/full/0/default.jpg```

![Diadem 1](https://leszimmermann.github.io/digitales-storytelling/img/umsetzung/Diadem-1.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/umsetzung/Diadem-1.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

2. Nun bearbeiten wir die URL und ersetzen das erste ‘full’ durch Koordinaten eines Bildausschnitts ‘810,750,450450’ - dadurch wird uns anstelle des gesamten Bildes ein bestimmter Ausschnitt angezeigt: ```https://ids.si.edu/ids/iiif/NMAH-ET2011-40071/full/full/0/default.jpg``` ->
```https://ids.si.edu/ids/iiif/NMAH-ET2011-40071/810,970,450,450/full/0/default.jpg```

![Diadem 2](https://leszimmermann.github.io/digitales-storytelling/img/umsetzung/Diadem-2.jpg)
<p style="font-size: 0.8em;margin-top:-15px;"><a href="https://leszimmermann.github.io/digitales-storytelling/img/umsetzung/Diadem-2.jpg" target="_blank" rel="noopener noreferrer">&#128269; Vergrößern</a></p>

Unter folgendem Link gibt es die Möglichkeit dies weiter auszuprobieren: [https://www.learniiif.org/image-api/playground](https://www.learniiif.org/image-api/playground).
Alle Möglichkeiten der Anpassung finden wir in der [IIIF-Dokumentation](https://iiif.io/api/image/2.1/).

Nun haben wir gesehen, wie IIIF arbeitet. Ein bißchen kompliziert für den Anfang? Keine Sorge: Da wir für die Erstellung unserer Digital Story den Viewer Storiiies benutzen, müssen wir die gewünschten Bildkoordinaten gar nicht selbstständig eingeben – das erledigt der Viewer für uns sozusagen im Hintergrund.

## Weblinks
- [Einführung IIIF (englisch)](https://youtu.be/wVjrqsqzwNI)
- [Einführung IIIF (deutsch)](https://av.tib.eu/media/34932)
- [Warum IIIF?](https://blog.cogapp.com/wtf-iiif-995ca796e654)
- [Workshop IIIF](https://training.iiif.io/iiif-online-workshop/)
- [Storiiies by Cogapp](https://storiiies.cogapp.com/)
- [Storytelling mit IIIF](https://canvas-panel.digirati.com/#/about)

---

Im nächsten Kapitel beschäftigen wir uns mit der technischen Umsetzung unserer Story:

<span class="fs-8">
[Zurück](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/technische-umsetzung/){: .btn .btn-outline .mr-2 } 
</span>
<span class="fs-8">
[Weiter](https://leszimmermann.github.io/digitales-storytelling/workshop/iiif/umsetzung-der-story-teil-1/){: .btn .btn-outline}
</span>