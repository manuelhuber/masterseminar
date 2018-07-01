## Erkennung von audiovisuellen Events in Überwachungskameraaufnahmen 

Manuel Huber

+++

![Surveillance Camera](https://i.ytimg.com/vi/htNfaaLu9aU/maxresdefault.jpg)

+++

![Flux Explained](https://imgs.xkcd.com/comics/machine_learning.png)

---

## AVC-Matrix

Audio-Video-Concurrency - Matrix

+++?image=presentation/overview.png&size=auto 90%

+++?image=presentation/AVC-Coupling.png&size=auto 90%

+++

![AVCM1](presentation/avc1.png)

+++

![AVCM1](presentation/avc2.png)

+++?image=presentation/AVC-Example.png&size=auto 90%

---

## TAPPMOG

Time-Adaptive (Per-Pixel) Mixture Of Gaussians

+++

Ist die Gaußverteilung 
- ein Treffer:
  - Erhöhe Gewichtung, passe Mittelwert an, verringere Standardabweichung
  - Markiere Messwert als Vordergrund, wenn Summe der Gewichte > T 
- kein Treffer:
  - Verringere Gewichtung

+++ 
  
Ist keine Gaußverteilung ein Treffer:
- Markiere Messwert als Vordergrund
- Ersetze Gaußverteilung mit geringstem Gewicht
  
  
