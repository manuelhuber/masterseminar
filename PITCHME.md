## Erkennung von audiovisuellen Events in Überwachungskameraaufnahmen 

Manuel Huber

+++

![Surveillance Camera](https://i.ytimg.com/vi/htNfaaLu9aU/maxresdefault.jpg)

+++

![Flux Explained](https://imgs.xkcd.com/comics/machine_learning.png)

---

# AVC-Matrix

Audio-Video-Concurrency - Matrix

+++?image=presentation/overview.png&size=auto 90%

---

TAPPMOG

Time-Adaptive (Per-Pixel) Mixture Of Gaussians

+++

Vergleiche jeden neuen Messwert mit absteigend mit jeder Gaußverteilung. Ist die Gaußverteilung 
- ein Treffer:
  - Erhöhe Gewichtung
  - Passe Mittelwert an, verringere Standardabweichung
  - Markiere Messwer als Vordergrund, wenn Summe der Gewichte > T 
- kein Treffer:
  - Verringere Gewichtung

+++  
  
Ist keine Gaußverteilung ein Treffer,
- Markiere Messwert als Vordergrund
- Entferne Gaußverteilung mit geringstem Gewicht
- Füge neue Gaußverteilung um den Messwert hinzu
  
  
