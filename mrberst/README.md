# 💥 Mr. Quiz – Die Familien-Spielshow

Ein Fragen-Generator für den Familienabend, für alle Altersgruppen.
Der Name der Show („MR. …“) und die Fotos werden auf dem Handy eingegeben und bleiben nur dort.

- **Großer roter Knopf:** Ein zufälliges Familienfoto zerplatzt in Puzzleteile, dahinter erscheint die nächste Frage.
- **Drei Fragearten** (125 Fragen) aus Tiere & Natur, Körper & Essen, Welt & Rekorde, Alltag & Kurioses:
  - 🔢 **Schätzfragen:** Das Handy geht reihum, jeder tippt geheim seine Zahl ein. Der Nächste bekommt 1 Punkt, ein Volltreffer 2 Punkte.
  - ⚖️ **Was ist mehr?** und 🤥 **Wahr oder Quatsch?**: Countdown, alle zeigen gleichzeitig (Finger/Daumen),
    dann auflösen und antippen, wer richtig lag (1 Punkt).
- **🎙️ Elternmodus (Quizmaster):** Mama oder Papa sieht Frage und Lösung sofort und liest vor. „🎲 Nächste Frage“ liefert eine zufällige Frage ohne Wiederholung,
  „🎲 Bunter Mix“ mischt alle Themen und Fragearten, alternativ ein einzelnes Thema. Die Lösung lässt sich verdecken (🙈), falls Kinder mitschauen.
- **🎲 Bunter Mix** gibt es auch im normalen Spiel: ein Tipp auf der Startseite schaltet alle Themen und Fragearten an.
- **Punkte sind optional:** „Ohne Punkte“ braucht keine Spielerliste – Schätzungen werden laut gesagt und direkt aufgelöst.
- **Jeder gegen jeden oder Teams**, endlos spielen, „🏁“ beendet die Show mit Siegerehrung.
- Punkte werden nicht gespeichert. Gemerkt werden nur Spielernamen, Showname, Auswahl und Fotos (alles nur auf dem Gerät).

## Eigene Fragen ergänzen

In `index.html` stehen oben die Fragen:

```js
["s","tiere","🐕","Wie viele Zähne hat ein erwachsener Hund?",42,"Zähne","Wow-Fakt …"],                 // Schätzfrage
["m","welt","Was ist höher?",["🗼","Eiffelturm","330 m"],["⛪","Kölner Dom","157 m"],0,"Wow-Fakt …"],  // Was ist mehr? (0 = links richtig, 1 = rechts)
["w","tiere","🐙","Ein Oktopus hat drei Herzen.",true,"Wow-Fakt …"],                                    // Wahr (true) oder Quatsch (false)
```

Nach Änderungen in `sw.js` die Versionsnummer bei `CACHE` erhöhen.
