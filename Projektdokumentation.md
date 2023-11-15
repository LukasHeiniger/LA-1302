# Projekt-Dokumentation

Mirhan Özden, Lukas Heiniger Mirhan

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|       | 0.0.1   | ✍️ Jedes Mal, wenn Sie an dem Projekt arbeiten, fügen Sie hier eine neue Zeile ein und beschreiben in *einem* Satz, was Sie erreicht haben. |
|       | ...     |                                                              |
|       | 1.0.0   |                                                              |

## 1 Informieren

### 1.1 Ihr Projekt

Unser Projekt ist ein 3D-Survival Videospiel. welches wir in Unity programmieren.

Unser Ziel ist es, ein Spiel zu programmieren, welches man selber ein paar Stunden lang privat spielen würde, ohne dass es langweilig wird.
Dabei wollen wir folgende Sachen lernen: Wie man Verschiedene Waffen einfügt, wie man in 3D Gegner einfügt, wie man Gegenstände aufheben kann etc. 
Auch wollen wir lernen wie man in 3D alles programmiert, wie wir es bei der 2D gemacht haben.
### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    | muss                |  funktional    | Als ein Spieler möchte ich mich bewegen können, um vor den Zombies wegzurennen |
| 2  |  muss                 | funktional      | Als ein Spieler möchte ich Springen können, damit ich auf höher gelegene Positionen springen kann.                                   |
| 3    | kann                | funktionel     | Als ein Spieler möchte ich mich ducken können, damit ich durch kleine Gänge gehen kann.|
| 4  |  muss               | funktional     | Als ein Spieler möchte ich Zombies, damit ich vor dennen wegrennen kann oder diese besiegen.                                   |
| 5    |  muss               | funktional     | Als ein Spieler möchte ich Waffen, damit ich mich gegen die Zombies wehren kann.|
| 6  | muss                | funktional     | Als ein Spieler möchte ich mir ein Unterschlupbauen können, damit ich mich vor den Zombies verstecken kann.                                   |
| 7   |  kann             |  funktional   | Als ein Spieler möchte ich Items herstellen, damit ich mich gegen die Zombies wehren kann. |
| 8  | kann                | funktional     | Als ein Spieler möchte ich Items aufsammel können, damit ich Sachen herstellen kann.                                   |
| 9    |  muss               |  funktional    | Als ein Spieler möchte ich Bäume und Steine abbauen, damit ich Ressourcen habe, um ein Haus zubauen. |
| 10  |kann                | qualität      |  Als ein Spieler möchte ich Animationen im Spiel, damit es schöner aussieht.                                  |
| 11   |  kann               | qualität     | Als ein Spieler möchte ich Sounds haben, damit die Welt sich realistischer anfühlt. |
| 12 | muss                | Randanforderung     | Als ein Spieler möchte ich eine Karte haben, damit ich auf dieser Spielen kann.                                    |
| 13   | muss                | funktional     | Als ein Spieler möchte ich essen und trinken, damit es noch schwieriger ist zu überleben. |
| 14 |   kann              | funktional     |  Als ein Spieler möchte ich ein Fortbewegungsmittel verwenden, dmait ich mich schneller und sicherer fortbewegen kann.                                  |
| 15   |  kann               | funktional     | Als ein Spieler möchte ich Erfahrung (XP) sammeln, damit ich meinen Charakter verbessern kann. |
| 16 |   kann              | funktional     |  Als ein Spieler möchte ich mein Spiel speichern und laden können, damit meine Welt gespeichert ist und ich sie diese ein anderes Mal wieder starten kann  |       




✍️ Jede User Story hat eine ganzzahlige Nummer (1, 2, 3 etc.), eine Verbindlichkeit (Muss oder Kann?), und einen Typ (Funktional, Qualität, Rand). Die User Story selber hat folgende Form: *Als ein 🤷‍♂️ möchte ich 🤷‍♂️, damit 🤷‍♂️*.

### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  | Spiel wurde gestartet             |  W/A/S/D       | Spieler bewegt sich                  |
| 2.1  | Spiel wurde gestartet             | Space        |  Spieler sprint                 |
| 3.1  | Spiel wurde gestartet               |  CTRL       |   Spieler duckt sich                |
| 4.1 | Spieler erkundet sich             | /         |      Zombies sind vorhanden             |
| 5.1  | Waffe wird ausgerüstet             |   Linksklick      |     Waffe feuert              |
| 5.2 |  Waffe wurde benutzt            |    R     |     Waffe wird nachgeladen, wenn Mun. vorhandenist              |
| 6.1  | Materialien sind vorhanden             |   ?      |   Unterschlupf kann gebaut werden                |
| 7.1  |  Materialien sind vorhanden            |  I       |      Inventar öffnet sich mit der möglichkeit Items herzustellen.             |
| 8.1  |  Item liegt auf dem Boden            |    E     |       Objekt wird aufgehoben und im Inventar gespeichert            |
| 9.1  | Baum ist vorhanden              | Linksklick mit Axt        |       Baum fällt um Ressourcen werden dem Spieler hinzugefügt            |
| 9.2  | Stein ist vorhanden             | Linksklick mit Spitzhacke        |   Stein wird abgebaut und Ressourcen werden dem Spieler hinzugefügt                |
| 10.1  | Onjekt mit Animationen ist vorhanden             |   /      |    Animationen werden abgespielt               |
| 11.1  | Objekt welches Sound abspielen kann ist vorhanden             |  /       |   Sound wird abgespielt                |
| 12.1  | Spiel wird gestartet             |     /    |      Karte ist vorhanden             |
| 13.1  |   Der Spieler hat Essen oder Trinken           |  Item wird gegessen       |     Hunger oder Durst wird gestillt              |
| 14.1  |  Der Spieler hat ein Fortbewegungsmittel gefunden            |   W/A/S/D      |   Fortbewgungsmittel bewegt sich                |
| ...  |              |         |                   |
| ...  |              |         |                   |
| ...  |              |         |                   |
| ...  |              |         |                   |

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, die der Testfall abdeckt, und `m` von `1` an nach oben gezählt. Beispiel: Der dritte Testfall, der die zweite User Story abdeckt, hat also die Nummer `2.3`.

### 1.4 Diagramme

✍️Fügen Sie hier ein Use Case-Diagramm mit mindestens 3 Anwendungsfällen ein; und eine Skizze davon, wie Ihre Netzseite aussehen sollte.

## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 22.11      |  Mirhan         |  Spieler soll sich bewegen können            |    45 Minuten           |
| 2.A  | 22.11      |  Mirhan         |   Spieler soll springen können           |    45 Minuten           |
| 3.A  |  22.11     |  Mirhan         |   Spieler soll sich ducken können           |  20 Minuten             |
| 4.A  |  22.11     |   Lukas        |  Besiegbare Zombies            |  90 Minuten             |
| 5.A  |  22.11     |  Lukas         |  Waffen            |  90 Minuten             |
| 6.A  |  29.11     |  Lukas         |  Basis bauen            |  120 Minuten             |
| 7.A  |  29.11     |  Mirhan        |  Items herstellen            |  120 Minuten             |
| 8.A  | 29.11      |  Lukas         |  Items aufsammeln            | 90 Minuten              |
| 9.A  | 29.11      |  Mirhan         |   Bäume/Steine abbauen           |  120 Minuten             |
| 10.A  |  6.12     |  Lukas         |  Animationen einbauen            | 60 Minuten              |
| 11.A  |  6.12     |  Mirhan         | Sounds einbauen             |  90 Minuten             |
| 12.A  | 6.12      |  Lukas         | Karte             | 60 Minuten              |
| 13.A  | 6.12      |  Mirhan         |  Essen & Trinken            |  90 Minuten             |
| 14.A  | 6.12      |  Lukas         |   Fortbewegungsmittel           | 90 Minuten              |




Total: 

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, auf die sich das Arbeitspaket bezieht, und `m` von `A` an nach oben buchstabiert. Beispiel: Das dritte Arbeitspaket, das die zweite User Story betrifft, hat also die Nummer `2.C`.

✍️ Ein Arbeitspaket sollte etwa 45' für eine Person in Anspruch nehmen. Die totale Anzahl Arbeitspakete sollte etwa Folgendem entsprechen: `Anzahl R-Sitzungen` ╳ `Anzahl Gruppenmitglieder` ╳ `4`. Wenn Sie also zu dritt an einem Projekt arbeiten, für welches zwei R-Sitzungen geplant sind, sollten Sie auf `2` ╳ `3` ╳`4` = `24` Arbeitspakete kommen. Sollten Sie merken, dass Sie hier nicht genügend Arbeitspakte haben, denken Sie sich weitere "Kann"-User Stories für Kapitel 1.2 aus.

## 3 Entscheiden

✍️ Dokumentieren Sie hier Ihre Entscheidungen und Annahmen, die Sie im Bezug auf Ihre User Stories und die Implementierung getroffen haben.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |       |           |               |                   |
| ...  |       |           |               |                   |

✍️ Tragen Sie jedes Mal, wenn Sie ein Arbeitspaket abschließen, hier ein, wie lang Sie effektiv dafür hatten.

## 5 Kontrollieren

| TC-№ | Datum | Resultat | Tester |Testumgebung|
| ---- | ----- | -------- | ------ | ---------|
| 1.1  |       |          |        ||
| ...  |       |          |        ||

✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

## 6 Auswerten

✍️ Fügen Sie hier eine Verknüpfung zu Ihrem Lern-Bericht ein.
