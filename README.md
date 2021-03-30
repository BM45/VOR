# VOR

![vor](https://github.com/BM45/VOR/blob/main/pics4www/VOR.jpg)

VOR - ein experimenteller Radiokompass für gerichtete Drehfunkfeuer (VORs) für PC und Raspberry auf Basis eines Software-Defined-Radio

### Was sind VORs?

VORs sind Funkstationen die zur Navigation vornehmlich im UKW-Flugfunkbereich operieren. Im Gegensatz zu nicht-gerichteten Funkfeuern (u.a. NDBs auf Langwelle), die auf Seiten des Empfängers zum Beispiel mit einer sich drehenden Antenne angepeilt werden müssen, senden VORs die relative Richtung Sender<->Empänger "codiert" mit, können also mit einem einfachen Rundstrahler wie einer Teleskopantenne empfangen werden. Typische VOR-Sendestationen sehen so aus.

![vor2](https://github.com/BM45/VOR/blob/main/pics4www/vorreal.jpg)

VORs befinden sich in der Nähe wichtiger Flugrouten oder an Flughäfen. Über dieses VORs kann man seine Position auch ohne Satellitennavigationssystem wie GPS oder GALILEO gut und ausreichend genau bestimmen. Ein Flugzeug kann sich also entlang dieser Flugfunkfeuer bis zu seinem Ziel hangeln. Aktive VORs findet man in Flugkarten eingezeichnet, diese gibt es für die eigene Region zum Beispiel unter skyvector.com . Hier ein Kartensusschnitt mit VORs um Frankfurt/Main.

![vor3](https://github.com/BM45/VOR/blob/main/pics4www/skyvector_com.jpg)

### Wie ist das Signal eines VOR aufgebaut?

Um die Funktionsweise eines VOR zu verstehen, schaut man sich am Besten das Signalspektrum einer solchen Station an.

![vor4](https://github.com/BM45/VOR/blob/main/pics4www/spectrum_vor.jpg)

Das Sendesignal eines VOR besteht empfängerseitig aus zwei 30 Hz Signalen. Eines in Trägerlage und eines auf einem 9960Hz Unterträger. Ein 30Hz Signal erscheint im Empfänger immer dann, wenn das Richtfunkfeuer wie ein Leuchtturm in Richtung Norden (0°) "leuchten" würde. Das zweite 30-Hz Signal ist eine Richtungskomponente, die Empfängerseitig phasenschoben aufgenommen wird. Diese Richtungskomponente ist mit dem 0°-Nordsignal synchronisiert. Durch die Messung des Phasenversatzes beider 30Hz-Signale (die Phasenverschiebung kann ja nur zwischen 0° und 360° sein) erhält man die Richtungsinformation Sender<->Empfänger.

![vor5](https://upload.wikimedia.org/wikipedia/commons/d/d1/VOR_principle.gif)
