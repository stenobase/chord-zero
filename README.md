![CHORD ZERO](https://user-images.githubusercontent.com/461132/187019809-5aaccf27-c189-4561-801b-86f32a59df2b.jpg)

# CHORD ZERO Stenographic Keyboard

CHORD ZERO is a stenographic keyboard that can be used with
[Plover](https://www.openstenoproject.org/plover/) or any other application
that supports the [TX
Bolt](https://docs.qmk.fm/#/feature_stenography?id=tx-bolt) or
[GeminiPR](https://docs.qmk.fm/#/feature_stenography?id=geminipr) protocol.

## Build your own

### Create gerber files and order a PCB

The easiest way to create gerber files is with
[KiKit](https://github.com/yaqwsx/KiKit); and the easiest way to install
`KiKit` is with [pipx](https://pypa.github.io/pipx/):

```
$ pipx install kikit --system-site-packages
$ kikit fab <your_fab_of_choice> zero.kicad_pcb gerbers
```
This creates `gerbers/gerbers.zip`.  Use this file to order PCBs the same way
as you would usually do.

### Assembly

You will need the following parts:

1. 30x MX compatible switches
1. 30x key caps
1. 30x `1N4148W` (or similar)
1. 1x Raspberry Pi Pico
1. 1x `SMBJ5.0A` (or similar)
1. 2x `SK6812MINI` (optional)

You want linear switches with low actuation force. Gateron clears are a good
option.

You want key caps that minimize the gap between top and bottom row. Cherry
R2/R3 or OEM R3 are good options.

### Firmware

[Firmware and instructions are available here.](https://github.com/sol/qmk_firmware/tree/chord/keyboards/chord/zero#chord-zero-stenographic-keyboard)

## LICENSE

The CHORD ZERO Stenographic Keyboard is open source hardware.  You are
encouraged to produce your own keyboard based on the documentation and design
files of this project.  You are also encouraged to study and modify the design
and create derivatives.

- All documentation and design files of this project are released under the
  [CERN-OHL-S](LICENSE).
- Some of the used 3D models are licensed under the [MIT
  license](https://github.com/foostan/kbd/blob/master/LICENSE).
- The default firmware for this project is [QMK](https://qmk.fm/).  QMK is
  released under the terms of the [GNU General Public License, version
  2](https://qmk.fm/license/).
- All contributions to QMK that are specific to this project are released under
  the same terms as QMK itself.

<p align="center"><a href="https://certification.oshwa.org/de000129.html" title="OSHWA CERTIFIED DE000129"><img alt="OSHWA CERTIFIED DE000129" width="150" height="110" src="https://user-images.githubusercontent.com/461132/187019779-e19730fe-32b9-4ee0-ad52-3836fd8bb831.png"></a></p>
