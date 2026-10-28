# Drucken

PLA, 0,2 mm Schicht, 4 Wände, 5 Boden-/Deckschichten, 40 % Füllung. Keine Stützen außer beim Display-Gehäuse. Teile nicht drehen, die Ausrichtung in den Dateien passt.

In jedem Ordner liegt eine `.3mf`, in der alles schon angeordnet ist. Teile mit `_x2` im Namen werden zweimal gebraucht und sind in der `.3mf` doppelt drin.

Mein Drucker druckt ziemlich maßgenau. Die Röhrchen und die Schiebeteile sind im Original mit Übermaß konstruiert, deshalb habe ich bei diesen Teilen im Slicer eine X-Y-Konturkompensation von −0,1 mm gesetzt (Rechtsklick auf das Teil → Prozesseinstellungen → Qualität → Präzision). Bei anderen Druckern evtl. nicht nötig.

## 1 – Grundplatte
- base_plate_plc

## 2 – Shield, Rear Body, Front Body
- scale_shield_plc – Brim
- rear_body
- front_body_windowed

## 3 – Adapterplatte
- adapter_plate – Brim optional
- adapter_plate_lettering – gehört zur Adapterplatte (zweite Farbe). In der .3mf schon als Teil im selben Objekt.
- front_body_cover

## 4 – Behälter, Becher, Display
- hopper_base_60x2
- hopper_cap_60x2
- powder_cup_body
- display_body – Stützen nur auf dem Bett

## 5 – Innenteile
- pulley_40t_x2
- Front/RearVolumeReductionInsert Top + Bottom
- left/right_servo_hanger, left/right_shutter, spur_gear_x2
- front_discharger_mount, rear_discharge_mount
- display_bracket, case_rear_bracket

## 6 – Röhrchen, Waagenteller, Gehäuse
- large_rotary_tube – Kompensation −0,1, Naht zufällig
- small_rotary_tube_low_flow – Kompensation −0,1, Naht zufällig, Brim
- weighing_pan_plc
- case_bottom, case_top – Brim
- rear_body_interface – Kompensation −0,1
- rear_discharger_cup – Kompensation −0,1
- feeder_plug_x2

## 7 – Display-Front, Türen, Kleinteile
- display_front + display_front_lettering (zweite Farbe, schon als Teil im Objekt)
- front_rear_door_x2 – Kompensation −0,1
- front_window – Kompensation −0,1
- rear_discharger_sliding_door – Kompensation −0,1
- rear_discharge_cup_ring
- powder_cup_handle

## 8 – Behälterrohr
- hopper_tube (Ø 60,3 × 2,35 × 150 mm) – kein Vasenmodus, 6 Wände

## Einsätze und Schrauben (zusätzlich zur Original-Stückliste)
- 32 Gewindeeinsätze M3×5×4: Shield 12, Rear Body 8, Front Body 6, Display-Halterung 4, Becherring 2
- Display-Halterung an die Adapterplatte: 2× M3×10 von unten
- Grundplatte auf die Waage: 4× M4×12 Zylinderkopf
- Zusätzliche Shield-Befestigung: 2× M3×12 von unten, 2× M3×6 Linsenkopf von oben (versenkt)
