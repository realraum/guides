---
title: 3D-Druck Einführung (MK3.5 Drucker)
author: Elias Koller (elias)
---

# 3D-Druck Einführung (MK3.5 Drucker)
Der MK3.5 ist ein Upgrade vom MK3S. Der Drucker ist fast baugleich zum MK4S, bis auf
- Extruder Bauweise anders d.h.:
  - Andere Nozzles
  - Bed Leveling anders
  - Ist dadurch langsamer als der MK4S
- Andere (nicht ganz so genaue) Stepper-Motoren

Bitte [MK4 Instructions](./MK4S.md) lesen. Falls Einschulung zum MK4 und Zugang schon vorhanden, kann der MK3 auch nach dem lesen dieser Anleitung verwendet werden.

## Bed Leveling (!!!WICHTIG!!!)
- Der Prusa MK3.5 misst beim bed leveling, im gegensatz zum MK4, den Abstand zum printbed induktiv, NICHT zum sheet durch abtasten.
- Deshalb muss VOR (nacher geht nicht) jedem Druck sichergestellt werden, dass das richtige sheet eingestellt ist (steht rechts unten am LCD), wenn nicht unter Control => Sheet Profile ändern.
- Alle print sheets im R3 sind mit dem richtigen sheet profile beschriftet und kalibriert.
  - Sollte der Abstand von Nozzle zu Sheet nicht passen, oder ein neues Sheet hinzugefügt werden, bitte  Settings -> Hardware -> Steel Sheets -> [Sheet Name] -> First layer calibration durchführen und den Anweisungen folgen.
- WENN DAS FALSCHE SHEET EINGESTELLT IST, KANN DER DRUCKER / DAS SHEET BESCHÄDIGT WERDEN ODER DER DRUCK HAFTET NICHT UND SCHLÄGT FEHL!!!

## Nozzle
Momentan gibt es nur die 0.4mm brass-nozzle. Die MK4S Nozzles sind nicht kompatibel. Bitte mit dieser KEINE ABRASIVEN MATERIALIEN drucken (z.B. Carbon-Fiber oder Metallhaltige Filamente).

### Nozzle muss getauscht werden
TL;DR: Bitte nicht selber machen und Elias fragen, wenn es ein Problem mit der Nozzle gibt
- Ist viel aufwändiger als beim MK4, siehe https://help.prusa3d.com/article/changing-or-replacing-the-nozzle-mk2-5-s-mk3-s-mk3-5-s_2069 $\qrcode[height=20mm]{https://help.prusa3d.com/article/changing-or-replacing-the-nozzle-mk2-5-s-mk3-s-mk3-5-s_2069}$
- Filament muss entfernt und nozzle muss aufgeheizt sein, um sie zu tauschen (man verbrennt sich leicht)
- Es muss ein kleiner Spalt zwischen dem Heizelement und der Nozzle sein (falls nicht rinnt das Filament oben raus -> Extruder wird kaputt)
- Es müssen nach dem Nozzle-Change sheet profiles für alle Sheets im R3 manuell neu kalibriert werden (dauert ca 2h).

## Slicing im Prusa-Slicer

### Setup
- Menü > Konfiguration > Konfigurations-Assistent -> Prusa Research -> MK3.5/MK3.5S: 0.4mm
- Sonst gleich wie [MK4 Instructions](./MK4S.md)

## Kosten / Material
Die Preise sind identisch zum MK4 (1ct Maintenance + Filamentpreis), bitte für diesen Drucker in die Elias Spendenbox werfen oder Bankdaten erfragen.
