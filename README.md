# Orca Slicer Profiles — Ender 3 / BTT SKR Mini E3 V3.0

## Printer
- Ender 3 with BTT SKR Mini E3 V3.0 (STM32G0B1)
- Hotend: Red Lizard K1-M
- Extruder: Orbiter 1.5 (direct drive)
- Cooling: Hero Me 7 dual 5015
- Probe: BLTouch
- Input shaper: X=EI@113Hz, Y=ZV@49Hz

## Print Profiles

| Profile | Layer | Use |
|---|---|---|
| 0.08mm Extreme Quality | 0.08mm | Max detail, tight tolerance parts |
| 0.12mm High Quality | 0.12mm | Detailed visual parts |
| 0.16mm Standard | 0.16mm | Everyday quality |
| 0.20mm RedLizard K1M | 0.20mm | Fast quality |
| 0.24mm Draft | 0.24mm | Prototypes |
| 0.28mm Super Draft | 0.28mm | Quick functional parts |

All profiles include XY compensation calibrated to this printer:
- `xy_contour_compensation: 0.17mm`
- `xy_hole_compensation: 0.54mm`

## Installation

### Mac
```
cp process/*.json ~/Library/Application\ Support/OrcaSlicer/user/default/process/
cp machine/*.json ~/Library/Application\ Support/OrcaSlicer/user/default/machine/
```

### Windows
```
copy process\*.json %APPDATA%\OrcaSlicer\user\default\process\
copy machine\*.json %APPDATA%\OrcaSlicer\user\default\machine\
```

### Linux
```
cp process/*.json ~/.config/OrcaSlicer/user/default/process/
cp machine/*.json ~/.config/OrcaSlicer/user/default/machine/
```

Restart Orca Slicer after copying. Select **"Ender-3 Orbiter1.5 RedLizard K1M 0.4 nozzle"** as your printer.
