# Projekt-Dokumentation

Mirhan Özden, Lukas Heiniger Mirhan

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 15.11      | 0.0.1   | Informationen für das Projekt gesammelt.  |
| 22.11      | 0.0.2   |Angefangen mit dem Programmieren erster Prototyp des Zombies.                                                              |
| 29.11 -13.12      | 0.0.3   |   Weitere Arbeit am Projekt                                                           |
| 20.12     | 0.1.0   |   Erster Prototyp                                                       |
| 10.1     | 1.0.0   |   Grösstenteils fertiges Spiel                                                       |

## 1 Informieren

### 1.1 Ihr Projekt

Unser Projekt ist ein 3D-Survival Videospiel. Welches wir in Unity programmieren.

Unser Ziel ist es, ein Spiel zu programmieren, welches man selber ein paar Stunden lang privat spielen würde, ohne dass es langweilig wird. 
Dabei wollen wir folgende Sachen lernen: Wie man verschiedene Waffen einfügt, wie man in 3D Gegner einfügt, wie man Gegenstände aufheben kann etc. Zudem möchten wir die Fähigkeiten, die wir beim 2d Spiel erlernt habe, nun auch für 3d anwenden.
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



### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  | Spiel wurde gestartet             |  W/A/S/D       | Spieler bewegt sich                  |
| 2.1  | Spiel wurde gestartet             | Shift und W/A/S/D        |  Spieler sprint                 |
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
| 15.1 | Spieler tötet ein Zombie             | Töten des Zombies    |    Spieler erhält XP               |
| 15.2 | Spieler öffnet LVL System             | I        |  Spieler kann sein Charakter verbessern                 |
| 16.1  | Spieler spiel Spiel             | Spiel wird gespeichert        |   Spiel wurde abgespeichert                |
| 16.2 | Savegame vorhanden             | Spieler lädt Savegame        |      Spielfortschritt ist vorhanden             |


## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 22.11      |  Mirhan         |  Spieler soll sich bewegen können            |    50 Minuten           |
| 2.A  | 22.11      |  Mirhan         |   Spieler soll springen können           |    50 Minuten           |
| 3.A  |  22.11     |  Mirhan         |   Spieler soll sich ducken können           |  50 Minuten             |
|4.A   |22.11       |Mirhan           |Einen Cursor machen                          |15 Minuten|
| 5.A  |  22.11     |   Lukas        |  Besiegbare Zombies            |  90 Minuten             |
| 6.A  |  22.11     |  Lukas         |  Waffen            |  90 Minuten             |
| 7.A  |  29.11     |  Lukas         |  Basis bauen            |  120 Minuten             |
| 8.A  |  29.11     |  Mirhan        |  Items herstellen            |  120 Minuten             |
| 9.A  | 29.11      |  Mirhan         |  Items aufsammeln            | 120 Minuten              |
| 10.A  | 29.11      |  Mirhan         |   Bäume/Steine abbauen           |  120 Minuten             |
| 11.A  |  6.12     |  Lukas         |  Animationen einbauen            | 60 Minuten              |
| 12.A  |  6.12     |  Mirhan         | Sounds einbauen             |  90 Minuten             |
| 13.A  | 6.12      |  Lukas         | Karte             | 60 Minuten              |
| 14.A  | 6.12      |  Lukas         |  Essen & Trinken            |  90 Minuten             |
| 15.A  | 6.12      |  Lukas         |   Fortbewegungsmittel           | 90 Minuten              |
|16.A   |6.12       |Mirhan          |Inventarsystem machen|180 Minuten|
|17.A   |6.12       |Mirhan          |Gegenstände im Inventar sortieren können|120 Minuten
|18.A   |13.12      |Mirhan          |    Ein Text soll erscheinen, je nachdem welchen Gegenstand man anschaut             | 90 Minuten  |
| 19.A  | 20.12      |  Lukas         |  Lebensanzeige           |  45 Minuten             |
| 20.A  | 20.12      |  Lukas         |   Ausdaueranzeige           | 45 Minuten              |


## 3 Entscheiden

Wir haben uns nach dem Informieren und Planen dafür entschieden, das wir nur die wichtigsten Funktionen implementieren, da der rest sonst viel zu lange gedauert hätte.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |  22.11     |  Mirhan Özden         |   50 Minuten            |   40 Minuten                |
| 2.A  | 22.11       | Mirhan Özden          |    50 Minuten           |   40 Minuten                |
|3.A|22.11 |Mirhan Özden| 50 Minuten| 45 Minuten   |
|4.A|22.11|Mirhan Özden|10 Minuten|10 Minuten|
|5.A|22.11|Lukas Heiniger|90min|180min|
|6.A|22.11|Lukas Heiniger|90min|240min|
|7.A|29.11|Lukas Heiniger|120min|nicht angefangen|
|8.A|29.11|Mirhan Özden|120 Minuten| 200 Minuten (Funktioniert nicht ganz)|
|9.A|29.11|Mirhan Özden|120 Minuten|150 Minuten|
|10.A|29.11|Mirhan Özden|120 Minuten|(Wegen der Zeit nicht geschafft)|
|11.A|6.12|Lukas Heiniger|60min|60min||
|12.A|6.12|Mirhan Özden|90 Minuten|70 Minuten|
|13.A|6.12|Lukas Heiniger|60min|60min||
|14.A|6.12|Lukas Heiniger||||
|15.A|6.12|Lukas Heiniger||||
|16.A|6.12|Mirhan Özden|120 Minuten|200 Minuten|
|17.A|6.12|Mirhan Özden|120 Minuten|150 Minuten|
|18.A|13.12|Mirhan Özden|90 Minuten|120 Minuten|
|19.A|9.1|Lukas Heiniger|45min|90min|
|20.A|9.1|Lukas Heiniger|45min|90min|



## 5 Kontrollieren

| TC-№ | Datum | Resultat | Tester |Testumgebung|
| ---- | ----- | -------- | ------ | ---------|
| 1.1  | 10.01.24|  funktioniert        | Lukas       | Zuhause am Schreibtisch |
| 2.1  | 10.01.24|  funktioniert        | Lukas       | Zuhause am Schreibtisch |
| 3.1  | 10.01.24|  funktioniert        | Lukas       | Zuhause am Schreibtisch |
| 4.1  | 10.01.24|  ist vorhanden       | Lukas       | Zuhause am Schreibtisch |
| 5.1  | 10.01.24| funktioniert bis auf das wechseln         | Lukas       | Zuhause am Schreibtisch |
| 5.2  | 10.01.24| funktioniert         | Lukas       | Zuhause am Schreibtisch |
| 6.1  | 10.01.24| funktioniert nicht         | Lukas       | Zuhause am Schreibtisch |
| 7.1  | 10.01.24| funktioniert          | Lukas       | Zuhause am Schreibtisch |
| 8.1  | 10.01.24| funktioniert          | Lukas       | Zuhause am Schreibtisch |
| 9.1  | 10.01.24| nicht vorhanden        | Lukas       | Zuhause am Schreibtisch |
| 9.2  | 10.01.24| nicht vorhanden          | Lukas       | Zuhause am Schreibtisch |
| 10.1  | 10.01.24| ist vorhanden         | Lukas       | Zuhause am Schreibtisch |
| 11.1  | 10.01.24| ist vorhanden         | Lukas       | Zuhause am Schreibtisch |
| 12.1  | 10.01.24| ist vorhanden         | Lukas       | Zuhause am Schreibtisch |
| 13.1  | 10.01.24| nicht vorhanden         | Lukas       | Zuhause am Schreibtisch |
| 14.1  | 10.01.24| nicht vorhanden         | Lukas       | Zuhause am Schreibtisch |
| 15.1  | 10.01.24| nicht vorhanden         | Lukas       | Zuhause am Schreibtisch |
| 15.2  | 10.01.24| nicht vorhanden         | Lukas       | Zuhause am Schreibtisch |
| 16.1  | 10.01.24| nicht vorhanden        | Lukas       | Zuhause am Schreibtisch |
| 16.2  | 10.01.24| nicht vorhanden         | Lukas       | Zuhause am Schreibtisch |


Da wir nicht alles in der vorgegebene Zeit schaffen konnten haben wir uns auf die wichtigsten Funktionen fokussiert. Trozdem sind wir recht zufrieden mit dem Ergebnis


