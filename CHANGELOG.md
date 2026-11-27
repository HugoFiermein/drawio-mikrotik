# Changelog

Versions follow `MAJOR.MINOR.PATCH`: see *Versions* in [README](README.md).

## [1.5.0] (unreleased)

### Library
- Licence: CC BY-SA 4.0 (see README for what it means for diagrams); trademark notice for the MikroTik names and logo.
- One SVG per model in `svg/<category>/`.
- Categories: **Cloud Core Routers**, **Routers**, **Indoor Wireless**, **Switches**, **LTE/5G**, **IoT**, **60 GHz**, **RouterBOARD**.
- Built files in `library/`: one `.xml` per category.
- Library labels: commercial name first, service name in brackets, e.g. `hEX (RB750Gr3)`; models without a commercial name keep the service name. SVG file names stay by service name. Superscripts are written as plain digits (`hAP ac2`), years without brackets (`hEX S 2025`).
- One scale for every model: 1200 px = 210 mm (real proportions between devices).
- `vector-hq/` removed: previous library files stay available in releases v1.2–v1.4.1.

### New models
- **Cloud Core Routers:** CCR1009-7G-1C-1S+, CCR1009-7G-1C-1S+PC, CCR1009-7G-1C-PC, CCR1009-8G-1S-1S+PC, CCR1016-12G, CCR1016-12G_old, CCR1016-12S-1S+, CCR1036-12G-4S, CCR1036-12G-4S_old, CCR2216-1G-12XS-2XQ
- **Routers:** RB1100, RB1100AH, RB1100AHx2, RB1100AHx2-LM, RB1100Hx2, RB1200, RB2011iL-IN, RB2011iL-RM, RB2011iLS-IN, RB2011UiAS-IN, RB2011UiAS-RM, RB3011UiAS-RM, hEX (RB750Gr3), hEX S (RB760iGS), hEX S 2025 (E60iUGS), ROSE Data server (RDS2216-2XG-4S+4XS-2XQ, front and rear view), RB5009UG+S+IN (strict front view: the logo and the heatsink fins sit on the top cover and are not part of it)
- **Indoor Wireless:** hAP ax3 (C53UiG+5HPaxD2HPaxD, orthographic port-side view with antennas), hAP lite (RB941-2nD), hAP lite (RB941-2nD, old revision with micro-USB power), hAP ac lite (RB952Ui-5ac2nD), hAP ac (RB962UiGS-5HacT2HnT), hAP ac2 (RBD52G-5HacD2HnD-TC), cAP ac (RBcAPGi-5acD2nD), wAP ac (RBwAPG-5HacD2HnD)
- **LTE/5G:** Chateau LTE12 2025 (D53G-5HacD2HnD-TC&EG120K-EA, rear view with the antenna mount plate), Chateau 5G R17 ax (S53UG+5HaxD2HaxD-TC&RG650E-EU, rear view with ports and both antennas)
- **IoT:** KNOT LR9G (RB924iR-2nD-BT5&BG770A&R11e-LR9G, port side with the RS485 terminal and the LoRa SMA connector)
- **60 GHz:** LHG 60G (RBLHGG-60ad, front view of the dish)
- **Switches:** CRS812 DDQ (CRS812-8DS-2DQ-2DDQ-RM, front panel with 400G QSFP56-DD, 200G QSFP56 and 50G SFP56 ports), CRS317-1G-16S+RM, CRS326-24G-2S+RM, FiberBox (CRS105-5S-FB, front view and inner panel)
- **RouterBOARD:** RB450Gx4 (top view of the bare board: stylised traces, main components, PoE sticker on port 5)

### Reworked models
- **CRS326-24G-2S+RM**: adopted the approved reworked front panel and updated the Switches library entry; the editable SVG source is preserved unchanged.
- **CRS812-8DS-2DQ-2DDQ-RM**: refined the QSFP56 metal rims and latch colours, added notches to the SFP56 cage bridges, aligned the console with the management block and moved the CONSOLE/RESET labels.
- **Old hardware revisions:** models whose case changed between revisions now come in two files, the current one under the model name and the old one with the `_old` suffix (CCR1016-12G_old and CCR1036-12G-4S_old: DB9 console on a metal plate with hex standoffs, mono LCD, single PSU; RB941-2nD_old: micro-USB power).
- **CCR1009-7G-1C-1S+**: DB9 console redrawn in the library style (metal plate with hex standoffs, metal rim, dark D-body, 9 pins) instead of a bare trapezoid.
- **CCR1036-12G-4S**: RJ45 console in the same colour as the Ethernet ports; "Cloud Core Router" title in Rajdhani SemiBold with a slight slant, as on the case.
- **CCR1009-8G-1S-1S+, RB3011UiAS-RM**: graph removed from the screen; plain grey screen like the rest of the library.
- **RB941-2nD, RB951Ui-2HnD, RB952Ui-5ac2nD, RB962UiGS-5HacT2HnT, RBD52G-5HacD2HnD-TC, RB750Gr3, CSS326-24G-2S+RM**: embedded raster images removed; DC jack pin and reset hole redrawn as vectors; empty `<text>` removed.
- **CCR1009 PC family** (7G-1C-PC, 8G-1S-PC, 8G-1S-1S+PC, 7G-1C-1S+PC): lower vent teeth raised to the SFP cage top on both sides, as on the device; with an SFP+ cage the left slope moved so the cage no longer overlaps the vent frame.
- **CCR1009-8G-1S-PC**: short contacts in RJ45 ports; port LEDs as on the device (green left, yellow right); only PWR lit.
- **RB1100, RB1100AH**: added to the library from sources, with contacts in all 13 ports (opposite the latch; ETH11/12 latch up), port LEDs off with colour hint, only PWR lit.
- **RB2011iL-IN**: redrawn in the library's technique with the original geometry: soft gradients, port contacts, PoE-out marks, only PWR lit.

### Rules for all models
- Two case revisions are two files: current under the model name, old with `_old`.
- Screens are plain, without graphs.
- Only PWR is lit; other LEDs are off with a hint of their colour.
- RJ45: stepped latch, 8 short contacts inside.
- Labels centred on their element; pure vector: no raster, filters or `<text>`.

## [1.4.1] and earlier
See [releases](../../releases): v1.0 – v1.4.1.
