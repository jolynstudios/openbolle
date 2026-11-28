# openBolle case v1

The print files are in this folder:

| folder | what |
|---|---|
| [plates/](plates/) | ready-made 3MF print plates, one or three cases per plate |
| [stl/](stl/) | the individual parts as STL files |

The same files are also attached to each [release](https://github.com/jolynstudios/openbolle/releases): the 3MF plates and `openbolle-case-v1-stl.zip`.

## Printing

**Start with the two single-colour plates.** For one case, print [`plates/openbolle-case-v1-1x-zwart.3mf`](plates/openbolle-case-v1-1x-zwart.3mf) in black (front shell and board holder). Then print [`plates/openbolle-case-v1-1x-kleur.3mf`](plates/openbolle-case-v1-1x-kleur.3mf) in orange, blue or your chosen colour (rear shell and button). Use the matching `3x` pair for three cases. Each of these jobs uses one spool.

The plain `1x` and `3x` plates contain all four parts per case for a single-colour job. The `two-colour` plates contain the same parts with two colours assigned. Check the spool mapping in your slicer.

| plate | what |
|---|---|
| [`openbolle-case-v1-1x-zwart.3mf`](plates/openbolle-case-v1-1x-zwart.3mf) | one case: front shell and board holder, for black |
| [`openbolle-case-v1-1x-kleur.3mf`](plates/openbolle-case-v1-1x-kleur.3mf) | one case: rear shell and button, for your colour |
| [`openbolle-case-v1-3x-zwart.3mf`](plates/openbolle-case-v1-3x-zwart.3mf) | three cases: front shells and board holders |
| [`openbolle-case-v1-3x-kleur.3mf`](plates/openbolle-case-v1-3x-kleur.3mf) | three cases: rear shells and buttons |
| [`openbolle-case-v1-1x.3mf`](plates/openbolle-case-v1-1x.3mf) | one case, all four parts, one colour |
| [`openbolle-case-v1-3x.3mf`](plates/openbolle-case-v1-3x.3mf) | three cases, all parts, one colour |
| [`openbolle-case-v1-1x-two-colour.3mf`](plates/openbolle-case-v1-1x-two-colour.3mf) | one case, two colours assigned |
| [`openbolle-case-v1-3x-two-colour.3mf`](plates/openbolle-case-v1-3x-two-colour.3mf) | three cases, two colours assigned |

Use a clean 256 × 256 mm bed and the printer, plate and filament profiles that worked for your individual parts. Keep the supplied positions and orientations. Print by layer. Add a **5 mm outer brim** to the board holder and rear shell. In the preview, check the brims against your printer's usable area and leave room for any purge tower. If the tower will not fit, use the separate colour plates. Watch the holder's first layer. Stop if an edge lifts. You do not need supports.

The small screw spacers print separately. In [stl/](stl/), choose [`5_afstandsring_met_rand.stl`](stl/5_afstandsring_met_rand.stl) for a spacer with a snap-off brim, or [`5_afstandsring.stl`](stl/5_afstandsring.stl) for the plain one. Print three per case, plus any spares.

The four main parts are also there as individual STLs:

| file | part | what goes in it |
|---|---|---|
| [`1_voorschaal.stl`](stl/1_voorschaal.stl) | front shell | goes around the screen |
| [`2_achterschaal.stl`](stl/2_achterschaal.stl) | rear shell | GPS antenna, speaker, battery and USB-C socket, with the logo |
| [`3_bordhouder.stl`](stl/3_bordhouder.stl) | board holder | the board is screwed onto it |
| [`4_powerknop.stl`](stl/4_powerknop.stl) | power button | a cap over the board's power button |

## Parts list

Everything you need for one Bolle. No programming or soldering: everything uses small plugs and small screws. The full build guide (in Dutch) is at [openbolle.nl/docs/bolle/zelf-bouwen](https://openbolle.nl/docs/bolle/zelf-bouwen).

| part | details | buy |
|---|---|---|
| **Board** | Waveshare **ESP32-S3-Touch-AMOLED-1.75**, the version **with GPS** (the box says -G). A round screen with two microphones and connectors for a speaker and a battery. | [AliExpress (GPS version)](https://nl.aliexpress.com/item/1005009067973350.html) · [Amazon (complete set)](https://www.amazon.nl/dp/B0F7XWWMJW) · [Waveshare manual](https://docs.waveshare.com/ESP32-S3-Touch-AMOLED-1.75) |
| **GPS antenna** | A flat 27 × 27 mm square with a small plug. Comes with the GPS version. Without the antenna Bolle cannot find where it is. | included with the board |
| **Speaker** | Waveshare 8 Ω 2 W, type B: 30 × 20 × 6.8 mm, with a 2-pin 1.25 mm plug. | [Waveshare](https://www.waveshare.com/product/displays/accessories/speakers/8ohm-2w-speaker-b.htm) |
| **Battery** | A flat 3.7 V LiPo, size **803040** (40 × 30 × 8 mm), 1000 mAh, with a 2-pin 1.25 mm plug. | [Amazon](https://www.amazon.nl/dp/B0DPZNZ4D6) |
| **USB-C cable** | A short cable from USB-C to a USB-C socket with a screw-on plate (20 mm wide, holes 16 mm apart). This is how you charge Bolle from the back. | [AliExpress](https://nl.aliexpress.com/item/1005009100645444.html) |
| **Screws** | 8× 2 × 8 mm and 2× 2 × 4 mm. See [Screws](#screws) below. | [KING Microschroeven](#screws) |
| **Washers** | 3 small metal M2 washers. They go under the board's screws. | hardware store |
| **Filament** | PLA for indoor use. ASA or PETG if Bolle stays in the car, because they handle heat better. | |
| Phone (optional) | An iPhone for messages, calls and music | |

> [!CAUTION]
> **Check the battery polarity.** Another battery of the same size is fine, but **check which wire is plus** before you connect it. The red wire is plus. Compare it with the **+** at the battery connector on the board. Many cheap batteries have the plug the other way round. Connect it the wrong way and the board breaks.
>
> In shops the plug is called MX1.25, PH1.25 or Micro JST 1.25. It is 2 pins at 1.25 mm pitch.

The speaker has the same plug. For a speaker it does not matter which way round it goes in.

### Screws

Stainless steel screws from KING Microschroeven (Netherlands). They come in packs of 50 or 25, so one pack is enough for several Bolles.

| screw | per Bolle | where it goes | article no. | product page |
|---|---|---|---|---|
| Self-tapping screw for plastic, 2 × 8 mm, stainless steel (pack of 50) | 8 | 3 hold the board on the board holder (with a washer under each head), 5 close the case | A370-020-008 | [kingmicroschroeven.nl](https://www.kingmicroschroeven.nl/plaatschroef-voor-kunststof-2-x-8-mm-rvs-50-stuks.html) |
| Self-tapping screw for plastic, 2 × 4 mm, stainless steel (pack of 50) | 2 | hold the USB-C socket plate from the inside. Do not use longer screws, or the tip comes through the back. | A370-020-004 | [kingmicroschroeven.nl](https://www.kingmicroschroeven.nl/plaatschroef-voor-kunststof-2-x-4-mm-rvs-50-stuks.html) |
| Socket head cap screw M2 × 5, stainless steel A2, DIN 912 (pack of 25) | optional | not used in the current assembly steps | A310-020-005 | [kingmicroschroeven.nl](https://www.kingmicroschroeven.nl/bzk-inbusschroef-rvs-din-916-m2x5-25stuks.html) |

## Assembly

The step-by-step assembly is in the build guide (in Dutch): [openbolle.nl/docs/bolle/zelf-bouwen](https://openbolle.nl/docs/bolle/zelf-bouwen#in-elkaar-zetten).

Design © 2026 openBolle · [openbolle.nl](https://openbolle.nl) · [Licence](LICENSE)
