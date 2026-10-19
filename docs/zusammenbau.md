# Zusammenbau

Grundsätzlich wie im Original: https://github.com/eamars/OpenTrickler/blob/main/STL/OpenTrickler/README.md
Hier nur das, was bei meinem Aufbau anders ist oder wo ich hängen geblieben bin.

## Waage
- Glaskasten und die runde Edelstahlschale abnehmen, die vier Stifte rausschrauben.
- Grundplatte mit 4× M4×12 festschrauben, nur handfest.
- Waagenteller auf den Zapfen stecken. Er sitzt unten auf der Verdickung auf und darf die Grundplatte nirgends berühren.
- Einstellungen an der Waage (CAL beim Einschalten gedrückt halten, CAL = weiter, TARE = Wert ändern): C1=1, C2=1, C3=6, C4=33.

## Gewindeeinsätze
- M3×5×4, bei PLA mit ca. 200 °C einschmelzen, gerade und bündig setzen.
- Shield: 4 Originalsäulen oben und unten, 2 neue Säulen vorne oben und unten.

## Shield und Adapterplatte
- Shield mit 4× M3×12 an den Originalsäulen auf die Grundplatte schrauben, dazu 2× M3×12 von unten in die neuen Säulen.
- Freie Kabeldurchführungen im Shield mit den Feeder-Plugs zumachen.
- Adapterplatte mit den Originalschrauben auf das Shield, dazu 2× M3×6 Linsenkopf in die zwei versenkten Löcher vorne.

## Trickler
- Lager einpressen – mit Schraubstock oder den Einpresshilfen aus dem Original, nicht mit dem Hammer.
- Röhrchen: Zahnkranz-Ende hinten in den Rear Body. Das kleine Röhrchen (low flow) ist hinten zu, das gehört so.
- Riemen: 174 mm auf das große Röhrchen (rechter Motor), 166 mm auf das kleine (linker Motor).
- Hinter dem VolumeReducer-Deckel sitzt in beiden Bodies eine Tür. Vorne kommt zusätzlich die Fensterscheibe in die Front.

## Front Discharger Mount
Kleiner Trichter unter der Adapterplatte, genau unter dem Auslass. Weite Seite nach oben, Senkungen nach unten. Er wird mit 2× M3×10 von unten durch das vordere Lochpaar des Front Body geklemmt, das hintere Lochpaar bekommt 2× M3×8 ohne Mount.

## Elektronik
- Pico 2 WH aufs Board, TMC2209 richtig herum stecken (VM/EN beachten).
- J9: Jumper senkrecht für ein 1:1-Kabel.
- Servo-Stecker auf JST PH 2,54 umcrimpen (Werkzeug ist im Full Kit).
- Firmware, WLAN, Motortest, Servo-Gate: siehe OpenTrickler-RP2040-Controller.
- Feinmotor-Übersetzung 1.818 (V2).
