# ✨ Zauber-Quiz

Ein Familien-Quiz, das komplett auf dem Handy läuft –
ohne Konto, ohne Claude und nach dem ersten Öffnen auch ohne Internet.

- **Zwei Stufen:** 🌟 *Zauberlehrling* (leichtere Fragen, 3 Antworten, wird automatisch vorgelesen – für ca. 8–11 Jahre)
  und 🔮 *Meistermagier* (schwere Fragen, 4 Antworten – ab ca. 12 Jahren).
- **Themen:** 🌍 Allgemeinwissen, 🏰 Disney & Pixar, ⚡ Harry Potter, 📱 Influencer, 🎲 Bunter Mix – 5 Fragen pro Runde, 184 Fragen insgesamt.
  Das Influencer-Thema enthält auch Fragen zur Sicherheit im Netz (Werbung erkennen, Adresse geheim halten, Clickbait, Deepfakes).
- **Vorlesen:** 🔊-Knopf bei jeder Frage (nutzt die deutsche Stimme des Handys).
- **Zauberer-Avatar:** Pro richtiger Antwort 1 ⭐, bei 5 von 5 gibt es 3 ⭐ Bonus. Mit den Sternen schaltet man
  in der Garderobe Umhänge, Hüte (auch den Sprechenden Hut), Zauberstäbe, Tiere, Brillen und Hogwarts-Schals frei.
- **Familien-Duell:** 2–4 Spieler an einem Handy, reihum. Jeder bekommt Fragen in seiner eigenen Stufe,
  am Ende gibt es ein Siegerpodest. Weitere Spieler (z. B. Mama, Papa) legt man über „Neuer Zauberer“ an.

Spielstände werden nur auf dem jeweiligen Handy gespeichert (im Browser-Speicher).

## Aufs Handy bringen

Die App läuft über GitHub Pages: **https://t27t4hmhdz-crypto.github.io/zauberquiz/**
Die Adresse auf dem Handy öffnen und:

- **iPhone (Safari):** Teilen-Knopf → „Zum Home-Bildschirm“
- **Android (Chrome):** ⋮-Menü → „App installieren“ bzw. „Zum Startbildschirm hinzufügen“

Ab dann startet das Quiz wie eine normale App und funktioniert auch offline.

## Eigene Fragen ergänzen

In `index.html` steht oben die Liste `Q`. Eine Frage sieht so aus:

```js
["hp","l","🦉","Wie heißt Harrys weiße Eule?",["Hedwig","Errol","Krätze"],"Zusatzwissen nach der Antwort."],
```

Thema (`welt`, `disney`, `hp`, `influ`), Stufe (`l` leicht mit 3 Antworten, `s` schwer mit 4 Antworten), Emoji, Frage,
Antworten (die **erste ist immer die richtige**, die App mischt sie), Zusatzwissen.
Nach einer Änderung in `sw.js` die Versionsnummer bei `CACHE` erhöhen, damit die Handys das Update laden.
