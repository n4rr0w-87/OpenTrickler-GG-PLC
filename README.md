# OpenTrickler für die G&G PLC100B-C

Mein Umbau des [OpenTrickler](https://github.com/eamars/OpenTrickler) von eamars für die Feinwaage G&G PLC100B-C (100 g / 0,001 g).

Das ist **nicht** das Originalprojekt. Anleitung, Stückliste, Firmware und Support gibt es bei eamars:

- https://github.com/eamars/OpenTrickler
- https://github.com/eamars/OpenTrickler-RP2040-Controller

Hier liegen nur die Teile, die ich für meine Waage angepasst bzw. zusammengestellt habe.

## Was anders ist

- Grundplatte vom G&G JJ223BF Shield. Die PLC hat das gleiche Gehäuse und die gleichen Gewinde (165 × 155 mm, M4). Die zwei Löcher für den Pan-Cover vorne sind zu, dafür gibt es zwei zusätzliche Befestigungen für das Shield neben der Waagschalen-Öffnung.
- Shield (Dewey-Mod) mit zwei zusätzlichen Säulen vorne, Einsätze oben und unten.
- Eigener Waagenteller für den Zapfen der PLC (Bohrung 8,25 × 9,2 mm, Oberfläche bündig mit der Grundplatte).
- Alle Löcher für Gewindeeinsätze auf 4,4 mm verkleinert (M3×5×4). Die Originale haben 4,7 mm, das war mir zu locker.
- Schriftzug „OpenTrickler“ auf der Adapterplatte und „OpenTrickler / RESET“ auf der Display-Front (Schrift aus dem Memphis-Mod), jeweils als eigenes Teil für einen Farbwechsel.
- Display-Halterung mit Gewindeeinsätzen, wird von unten an die Adapterplatte geschraubt.
- Pulverbecher mit Gewindeeinsätzen für den Griff.
- Behälter-Unterteil und Deckel für ein Rohr mit 60 × 2 mm, passendes Rohr zum Drucken.
- Keine Haube (Pan-Cover), kein Plexiglas – Fenster und Rohr werden gedruckt.

## Hardware

- Waage: G&G PLC100B-C mit RS-232 (DB9 Buchse an der Waage)
- Controller: Mellow Pico Motor Expansion Board V2 (Full Kit), Raspberry Pi Pico 2 WH
- Kabel: DB9 Stecker/Buchse, 1:1 (Jumper J9 senkrecht)
- Waage einstellen: C1=1, C2=1, C3=6, C4=33
- Gedruckt auf einem Anycubic Kobra S1 in PLA

## Ordner

- `plates/` – eine Druckplatte pro Ordner, jeweils mit den STL-Dateien und einer fertig angeordneten `.3mf`
- `docs/drucken.md` – was auf welche Platte gehört und welche Einstellungen pro Teil
- `docs/zusammenbau.md` – meine Notizen zum Zusammenbau

## Danke

- eamars – OpenTrickler, A&D FX Shield, G&G JJ223BF Shield
- Dewey – Shield-, Adapterplatten- und Fenster-Mods, Gehäuse-Mod
- HayaminiNL – Controller-Gehäuse
- dirtbit – Display-Gehäuse
- Memphis – Schriftzug

Alle Teile stammen aus dem OpenTrickler-Repository (inkl. `CommunityContributions`) und sind von mir angepasst.

## Lizenz

GPL-3.0, wie das Original.

---

### English

My adaptation of [eamars/OpenTrickler](https://github.com/eamars/OpenTrickler) for the G&G PLC100B-C scale. Not the original project – see the link for the build guide, BOM and firmware. Print plates are in `plates/`, notes (German) in `docs/`. GPL-3.0.
