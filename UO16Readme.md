Hinweis: Beschreibung lieber in Raw Format betrachten zur besseren Lesbarkeit.

Aktueller Log:

Übersetzungsdinge // Text / Skript der nicht abgeändert werden kann:
================================================================
a) Die vier Vulkane können nicht der gegebenen Vegetation benannt werden.
b) Die vier BH Fabriken können nicht entsprechend der Vegetation benannt werden.
c) Es gibt drei unterschiedliche Brücken jedoch können die nicht separat bezeichnet werden.
d) Verweise der Bezeichnungen der verwendeten Waffen wird unter anderem kollektiv aber auch einzeln verwendet. Es wäre schön wenn man für jede Einheit auch separat deren Waffensystem bezeichnen könnte. 
e) Für alle co_empty_xy ist im internen Wiki -> CO aufgrund der Textstückelung ein fehlendes Leerzeichen vorhanden. Natürlich kann dies auch händisch über Qt Linguist eingefügt werden doch dann wird "Translation does not have same leading and trailing whitespace as the source text." angegeben. Auch wenn dies nicht von der Anwendung zu Problemen führt möchte ich es denoch genannt haben.
f) Im internen Wiki -> Others findet sich kein Skript mit "Damage Table" aka Schadenstabelle
g) Im Spielmenü -> Info -> Einheiteninfo: Die Bezeichnungen für die jeweiligen Spalten befinden sich nicht in der Sprachdatei (HP, Fuel, Ammo 1, Ammo 2)
h) Zum Start der Anwendung wird Text geladen (Lade xy...) welcher sich zu 60% nicht in der Sprachdatei befindet
i) Im Internen Wikipedia die Tags (sind in der Sprachdatei nicht enthalten) Hierzu gehören CO, Terrain, Building, Unit, Perk, Others, Action sowie Army
k) Karteneditor -> Skript editieren: Angegebene Bedingungen können nicht umgeschrieben werden (sind nicht in Sprachdatei vorhanden) analog hierzu auch Ereignisse. (befindet sich in ...\ingamescriptsupport\scripteditor.cpp)
l) Wenn kein CO gewählt wurde werden CO Informationen angegeben welche Texte angeben welche nicht abgeändert werden können (Unknown an mehreren Stellen)
m) In Spieleeinstellungen für Verbotene Aktionen werden hier fünf ohne weitere Beschreibung angegeben. Diese sind Gabe/Spezialgabe für CO1/2 aktivieren und Bordflugzeuge herstellen. Befinden sich auch nicht in der Sprachdatei.
n) Terrain Wasteland Forest aka Wald in Wüste beschreibt einen Text welcher separat einen Grüntext bildet. Dadurch ist keine Möglichkeit gegeben wie bei anderen eine genauere Aufsplittung von Normalen Text durch zu führen.


Grafische Dinge
===============
a) Die neu hinzugefügten Marineeinheiten (Kanonenboot, Missleboot, Torpedoboot, Zerstörer, Fregatte) sind ~50% kleiner als andere Einheiten. Einheitenanimationen unten rechts werden jedoch richtig dargestellt. // Die neu hinzugefügten Einheiten verfügen über ein zu großes Icon welches in ...\resources\images\units bearbeitet werden muss. Folgende Einheiten sind davon betroffen: gunboat mask, desroyer mask, frigate mask, torpedoboat mask, missleboat mask. (Angeboten kann nur eine verschlechterte 16x16 Grafik für jeweilige Einheiten)
b) Schwarze Geschütze, BH Fabrik, Schwarzer Laser, Schwarze Kanone, Laser, Vulkan usw. verfügen nach dem Originalspiel ein BH Icon mit einem Stop Symbol. Derzeit werden jedoch Stadtbilder verwendet. // Hintergründe für Black Hole Gebäude sind nicht vorhanden. Bei dem Versuch den Hintergrund hinzuzufügen wird dieser nicht vom Programm erkannt. Warum?
c) Betrifft wie in b) auch die Gebäude der Dark Matter / IDS (könnte aus Originalspiel entnommen werden)
d) Feuer hat Ebenenicon (kann aus Originalspiel entnommen werden)
e) Schön wäre den Abstand im internen Wiki für Einheiteninfo zu vergrößern (Zwischen Bewegung und Primärwaffe)
f) Im internen Wiki -> Aktionen werden Überschriften von Icons überdeckt. Es wäre gut das Icon links oder rechts neben der Überschrift anzeigen zu lassen.
g) Selbiges gilt auch für internes Wiki -> Army
h) Im Spiel -> Info -> Rechner: Es wäre schön wenn das Schließen Icon oben rechts vergrößert werden könnte. Meiner Meinung nach ist es sehr klein gehalten.
i) Manchmal sind Schriftzüge mit Umlauten nicht richtig dargestellt. Sobald man mit der Scrollbar die Position dieser abändert könnte es dazu kommen das dieser Fehler behoben wird.
j) Karteneditor -> Kampagneneditor: Schaltflächen sind unterschiedlich positioniert.
k) Ein größerer Abstand im Spieleeinstellungsmenü wäre zur besseren Übersicht gut.
l) Die Animation für das Raketen U-Boot steht still währenddessen die Animation der See normal abläuft.


Fehlende / Noch zu entwicklende Icons:
======================================
a) Teleportfläche hat Seeicon
b) Kraftwerk
c) Labor
d) Mine
e) Bohrinsel
f) Läuferstation
g) Plasma
h) Tor (orthogonal / vertikal)


Persönlich entschiedener aktueller Vorgang welchen ich mitteilen möchte (um ggf. auf Abänderungswünsche eingehen zu können):
===========================================
a) Alle neuen COs welche nicht im Originalspiel vorhanden waren wurden vom Namen nicht übersetzt.
b) Amber Corona => Unabhängige 13te Battalion, Teal Islands => Neolaurentianische Armee, Brown Desert => Zephyrianische Armee
c) Die meisten Fähigkeiten sind der Bezeichnung aus AWDS entnommen. Ggf. wurden Schwächungen entsprechend mit der Bezeichnung und einem - versehen.
d) Da die Bezeichnung Hovercraft aka Luftkissenfahrzeug zu lang ist habe ich mich für Luftkissen als Abkürzung entschlossen
e) Folgende Einheiten besitzen keinen Quelltext der die Einheit beschreibt (Iron Shield Gen. aka Mobiler Eiserner Vorhang, Repair Tank aka Reparaturpanzer, Missle Submarine aka Raketen U-Boot); Skript wurde nachverfolgt und manuell in jeweiligen Dateien nachgetragen, ausprobiert und auf Funktion in Anwendung überprüft
f) Beim gezündeten Raketensilo wir nicht nur die Rakete sondern auch die Absicherung mit abgeschossen (siehe Bild). Wurde manuell abgeändert.
g) Für die Aktion 1./2. CO einladen ist das dargestellte Icon besonders groß (wurde manuell behoben, die Grafik ist nicht standartmäßig 16x16 sondern in 48x48: wird verwendet aus ...\resources\images\game\co0 sowie co1).


Spielmechanische Dinge:
======================
a) Könnte im Karteneditor beim Karten speichern überschreiben eine zusätzliche Warnung hinzugefügt werden ob man auch wirklich die Datei überschreiben möchte?
b) Produktionen welche aus finanziellen Mitteln nicht möglich sind werden im Labor und Läuferstationen nicht angezeigt. (Üblicherweise werden diese mit roten Schriftzug markiert).
