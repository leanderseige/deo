The following text was publish 1993 and describes the functions of DeO. The
software is available under the GNU GPL V3 now, any license information below
is anvalid and was included for documentation only.

Leander Seige, 08.06.2020

###############################################################################

Anleitung zu DeO, Version 1.0, ©1993
von Leander Seige                                           6. Mai 1993

Bitte lesen Sie auf jeden Fall den Abschnitt `Allgemeines' am Ende dieser
Datei!

Vorstellung:
------------
DeO ist ein D_atenprogramm (für) e_xtragalaktische O_bjekte. Es wurde von mir
für eine Belegarbeit im Fach Astronomie erstellt.
Es zeigt die Positionsdaten (Rektaszension, Deklination und Entfernung) in
einem 3D-Koordinatensystem dar.
Zusätzlich können noch Bilder der Objekte aus dem Programm heraus angezeigt
werden. Es erkennt die Kürzel der Hubble-Sequenz. Weitere Funktionen später.

Das Programm war zwar ursprünglich für extragalaktische Objekte vorgesehen,
da aber lediglich die oben genannten Werte verwendet werden, können fast alle
astronomischen Objekte dargestellt werden.

Rechtliches u.s.w. siehe 'Allgemeines'.

Funktionen/Bedienung:
---------------------

1. Elemente am unteren Bilschirmrand :

 - Steuerkreuz (ganz rechts)
   Hier läßt sich daß 3D-Koordinatensystem um alle 3 Achsen drehen,
   um so den Blickwinkel verändern zu können. Die Pfeile nach oben
   und unten bestimmen den Winkel um die X-Achse. Die Pfeile nach
   links und rechts den um die Y-Achse. Die diagonalen Pfeile sind
   jeweils Kombinationen aus den beiden sich in der Ecke überschnei-
   denden Richtungen. Die großen Balcken oben und unten stehen für
   den Z-Winkel. Das Gadget in der Mitte mit dem 'R' setzt alle Winkel
   zurück auf 0.
   Alle Funktionen finden sich in dem Pull-Down-Menü 'Rotation' wieder.

 - Links vom Steuerkreuz sind 4 Gadgets im Zahlenangaben vorhanden.
   Die unteren 3 davon zeigen den momentanen Winkel jeweils um die
   X/Y/Z - Achse an. Sie besitzen keine aktive Funktion für den Be-
   nutzer.
   Das oberste mit der roten '10' zeigt den Betrag der Drehung pro
   Gadgetbetätigung an. Sie können diesen Wert verändern, indem Sie
   das Gadget anklicken und einen neuen Wert eintragen.

 - In der Mitte unten finden Sie 7 Textgadgets (rote Rahmen mit Text
   darin). Sie dienen zur Dateneingabe (Ancklicken+Schreiben)
   * Als erstes haben wir da ein relativ großes Gadget links oben.
     In dieses kommt der Name des Objekts. Soll ein IFF-Bild zu dem Objekt
     dargestellt werden, muß hier der Name (evtl. mit Pfad) OHNE das An-
     hängsel '.iff' des Bildes stehen. '.iff' wird zum Laden des Bildes an-
     gehängt. Das Gadget hat sonst weiter keine Funktion und wird auch nicht
     weiter vom Programm benutzt.
   * Rechts davon ist ein weiteres Gadget vorhanden, welches - ähnlich dem
     vorherigen - für Kennummern aus Katalogen vorgesehen ist (z.B. 'M521'
     oder 'NGC6256'). Der Inhalt wird vom Programm nicht ausgewertet.
   * Wieder rechts davon ist noch ein kleines Gadget - nur 3 Buchstaben -
     vorhanden, in welches eingetragen werden kann, um was es sich im Groben
     handelt. Folgendes wird erkannt:
     E0...E7   - ellyptische Galaxie      (Hubble-Sequenz)
     SO        - Sondergalaxie                   "
     Sa...Sc   - Spiralgalaxie                   "
     SBa...SBc -      "        mit Balken        "
     Irr       - Galaxie, nicht einzuordnen      "
     OS        - Offener Sternenhaufen
     KS        - Kugelsternhaufen
     HN        - Heller Nebel
     PN        - Planetarischer Nebel
     PLT       - Planet
     STR       - Stern
   In der zweiten Reihe sind 3 gleichgroße Gadgets vorhanden.
   * Das erste von links enthält die Rektaszension. Sie wird in Stunden und
     Minuten angegeben (1h=15°, 4'=1°). 0..24h ergeben einen Vollkreis von
     0..360°. Bei der Eingabe ist zu Beachten, daß zwischen der Stunden- und
     Minutenzahl min. ein anderer Buchstab/Leerzeichen steht. Die Angabe von
     Maßeinheiten o.ä. wirkt sich nicht aus.
   * Das Gadget in der Mitte der zweiten Reihe enthält die Deklination.
     Sie wird in Grad und Minuten angegben, wobei hier lediglich die Grad-
     zahl verwendet wird. Als einziges Gadget wird in diesem hier die Eingabe
     eines +/- Zeichens berücksichtigt. Fehlt es, wird + angenommen.
   * Das Gadget rechts in der zweiten Reihe enthält die Entfernung des Objekts
     in Parsec vom Koordinatenursprung. Folgt nach dem Zahlenwert (wahlweise
     mit Leerzeichen) ein M, so wird die Zahl mit 1Mio. , bei einem k mit
     1000 multipliziert.

  In keinem der 3 Gadgets in der zweiten Reihe werden irgendwelche Nachkomma-
  stellen beachtet. Sie können sogar zu Störungen führen.
  Beispiel :     Wert (z.B. aus Tabelle) = 4,4 Mpc
                 Eingabe (negativ. Bsp.) = "4,4 Mpc" oder "4.4 Mpc"
                 Deutung (negativ. Bsp.) = 4 pc
                 Eingabe (Richtig)       = "4400 kpc"
                 Deutung (Richtig)       = 4400*1000 pc = 4,4 Mpc !

   * Das größte Gadget in der dritten Reihe ist für Kommentare gedacht und
     fasst max. 90 Buchstaben.
 - Über diesem Textgadgetblock finden Sie 7 Gadgets, die mit Funktionen be-
   legt sind. Von links nach rechts:
   EXIT - Verläßt das Programm.
   LOAD - Laden einer Datei, die Mit DeO gesichert worden ist.
   SAVE - Speicher aller Objekte, die gerade verwaltet werden in einer
          Datei.
   CLR  - Löscht alle gerade verwalteten Objekte aus dem Speicher.
   ADD  - Fügt ein neues Objekt an, was dann mit entsprechenden Daten ver-
          sehen werden muß.
   DEL  - Löscht das aktuell dargestellte Objekt.
   TAKE - Wertet alle Objektdaten neu aus und überrechnte ihre Position im Ko-
          ordinatensystem.
 - In der linken unteren Ecke des Bildschirms finden Sie das Bild (schemat.)
   des aktuellen Objekts oder Symbole für Laden,Speicher,Animation u.s.w. ,die
   während dieser Vorgänge angezeigt werden.
 - Über diesem Bild sind die letzten beiden Gadgets.
   Da ja in den Textgadgets immer nur die Daten eines Objekts angezeigt werden
   können, ist es möglich, mit diesen Gadgets zwischen ihnen hin und her zu
   blättern. Das Bild links unten wird automatisch angepaßt. Ebenso der Würfel,
   der das aktuell angewählte Objekt umgibt und der 'Pfad', der die Position
   des Sterns verdeutlicht.
 - Links über diesen Gadgets finden Sie 4 farbig Rechtecke, die die farbl. Ab-
   stufung des Objekts je nach Entfernung vom Betrachter zeigen. Diese Abstuf-
   ung findet statt, um einen räumlichen Eindruck zu vermitteln und hat natülich
   nichts mit scheinb. Helligkeit o.ä. zu tun.
 - Rechts von diesen Rechtecken ist noch eine 'ZEIT'-Skala, die zeigt, wieviel
   Zeit noch vergeht, bis eine Animation (siehe unten) am Ende ist.

2. Das Koordinatensystem:

Zu Beginn sehen Sie das Koordinatensystem 'von vorn'. Die X-Achse ist waage-
recht von links nach rechts, ungefähr in der Mitte, zu sehen. Die Y-Achse ist
die Senkrechte. Auf die Z-Achse sieht man drauf. Sie zeigt geradezu auf den
Betrachter. Im Koordinatenursprung ist der Würfel zusehen, den man später von
Objekt zu Objekt 'springen' lassen kann. Der Pfeil an den Enden markiert die
'Plusseite' dar.
Der Pfad zeigt den Abstand der Objektposition vom Ursprung in jeder Dimension.

3. Pull-Down-Menüs:

>PROJEKT<
Laden/Sichern
   Nach evtl. Warnrequestern erscheint der Filerequester (asl.library), mit dem
   Sie Pfad und Dateiname auswählen bzw. CANCELn u.s.w. .
   DeO verwendet ein eigenes Dateienformat.
Über/Hilfe
   Stellt mit Hilfe des display-Befehls des CLI die Bilder ABOUT.IFF und
   HELP.IFF dar. Die Lösung mit dem display-Befehl ist zwar vielleicht nicht
   gerade die Eleganteste, aber sie hat den Vorteil, daß ich keine eigene
   Anzeigeroutine programmieren mußte, die sicher nicht sehr vielseitig aus-
   gefallen währe. So ist es möglich, eigene Anzeigeprogramme zu verwenden,
   die evtl. auch 24Bit-Karten o.ä. unterstützen, ich habe leider keine Ahnung,
   welche Möglichkeiten es da geben könnte, da ich keine Grafikkarte habe.
Bewegung
   Hier können Sie die Bewegungen, die Sie normalerweise mit dem Steuerkreuz
   ausführen lassen 'automatisieren'.
   Bei Anwahl des Menüpunktes erscheint ein Fenster, welches 6 Gadgets enthält.
   Die untersten beiden lassen die Animation beginnen (OK!) oder den Vorgang
   abbrechen (STOP).
   Die oberen vier sind Gadgets, in die Zahlen einzugeben sind. Als erstes von
   oben kommt das Gadget 'Takte'. Es gibt an, aus wieviel Schritten die Be-
   wegung bestehen soll. Danach folgen die 3 Gadgets, in denen angegeben wird,
   um wieviel Grad (+/-) sich der Darstellungswinkel pro Takt ändern soll.
Ende
   ...wie Gadget 'EXIT'. Es erscheint ein Requester und dann ist Schluß - oder
   auch nicht.

>ROTIEREN<
Als zweites Menü folgt eines, welches nochmals die Funktionen des Steuerkreuzes
verkörpert.

>OBJEKT<
Das dritte Menü birgt Funktionen zum aktuellen Objekt.

Bild zeigen
   Versucht mit Hilfe des Befehls 'display' welcher ab Kick. 2.04 zum OS ge-
   hört ein IFF-Bild des aktuellen Objekts zu zeigen. Das Textgadget für den
   Namen muß den richtigen Inhalt haben (siehe oben).
Verwaltung
   Dieses Untermenü enthält die Funktionen ADD,DEL und CLR, die schon als Gad-
   gets realisiert sind. Weiterhin ist eine Funktion zum Kopieren eines Ob-
   jekts enthalten, mit deren Hilfe eine Kopie des aktuell gezeigten Objekts
   erstellt wird. Dies ist nützlich, wenn Objekte eingegeben werden, die sehr
   ähnliche Daten aufweisen.
Übernehmen
   = Gadget TAKE.
Vorgänger/Nachfolger
   = die Gadgets zum Vor- und Rückblättern über dem Bild.
Zentrieren
   Setzt die Darstellungswinkel so, daß das aktuelle Objekt zum Betrachter
   zeigt.
Information
   Zeigt folgende Daten in einem eigenen Window (OK drücken um raus zu kommen):
    - In der oberen Hälfte sind die Konzentrationen der Objekte in einem Schema
      dargestellt.
      X/Y - Frontansicht
      X/Z - Draufsicht
      Y/Z - Seitenansicht (rechts)
      Die Konzentrationen werden in einem 8x8 Punkte Raster dargestellt.
      Um so heller ein Quadrat, um so mehr Objekte sind 'darin'.
      Die roten Kreise dienen dazu, die Ausmaße der gesamten 'Welt' dar-
      zustellen.

      Zugegebenermaßen hat diese Information sicher nicht die umwerfende
      Aussagekraft.
    - Unter 'Programminterna:' werden einige zusätzliche Informationen
      angezeigt:
      AX..AZ    - Darstellungswinkel in °
      X/Y (2D)  - effektive Positionsdaten in Pixel auf Bildschirm
      X..Z (3D) - Positionsdaten in dem von den Achsen gebildeten Quadrat von
                  320*320*320 Pixel
      Rekt./    - interpretierter und umgerechneter Inhalt der Textgadgets
      Dekl.       Rektaszension und Deklination
      Farbe     - aktuelle Darstellungsfarbe
      Entf.     - Entfernung statt pc in Pixel im Pixel-Würfel
Ausdrucken/Alles drucken
      Gibt entweder des aktuelle oder alle verwalteten Objekte auf einem
      angeschlossenen Drucker aus.

>GRAFIK<
Außer dem letzten können hier alle Punkt an- und ausgeschaltet werden.
Linien
      Erlaubt/Verbietet das Zeichnen des Würfels,der Achsen und des Pfads.
      Diese Funktion bringt einen Geschwindigkeitsgewinn (konstant) bei
      Animationen. Sie hat eine höhere Priorität als die folgenden 3 Punkte.
Achsen/Pfad/Cursor
      Hier können die entsprechenden Objekte aus- und eingeblendet werden.
Schattierung
      Abschaltung der Farbabstufung je nach Entfernung an/aus.
Falschfarben
      Umschaltung der sw-Palette auf eine rot-grüne.
Winkelwerte
      Schaltet die Nachzeichnung der Gadgets, die die Betrachtungswinkel an-
      zeigen ein/aus.
Invertieren
      Rotierung der Farbpalette (Nah zu Fern / Fern zu Nah).

>Prefs<
...hat derzeit nur einen Menüpunkt.
OS-Grafik
      Ermöglicht die Verwendung einer eigenen, schnelleren Blitterroutine,in
      der auch die Achsen von ihrer Tiefe her richtig dargestellt werden.
      Die Verwendung der Betriebssystemroutinen ist der Kompatibilität halber
      voreingestellt.

Allgemeines:
------------
Das Programm DEO ist Freeware.
Nur wenn folgende Bedingungen eingehalten werden, ist die Weitergabe und die
Benutzung für jedermann erlaubt und erwünscht:

 - Niemand darf durch die Weitergabe von DEO Gewinn machen.
 - Folgende Files müssen immer im gleichen Directory stehen:
     DEO
     DEO.dok
     ABOUT.iff
     HELP.iff
 - Der INHALT der Files DEO,ABOUT.iff und HELP.iff darf nicht verändert werden.
 - Das File DEO.dok darf nur im Bereich VOR dem Abschnitt 'Allgemeines' verän-
   dert werden. Mit Beginn des Abschnittes 'Allgemeines' darf kein Byte mehr
   verändert werden.

Alle weiteren Rechte werden beansprucht.

Für Hinweise auf Programmfehler bin ich jederzeit dankbar.
Ich bitte jeden, dem DEO gefällt, oder der DEO öfters benutzt, mir eine Ansichts-
karte zu senden (`Cardware').
Wer Probleme mit der Bedienung hat, kann sich natürlich auch bei mir melden.

Aufruf: Wenn es Computerclubs im Raum Leipzig gibt, die sich mit dem Amiga
        beschäftigen, bitte ich diese, sich bei mir zu melden, falls sie noch
        Mitglieder suchen.

Adresse:
Leander Seige
Friesenstraße 9
O-7125 Liebertwolkwitz
