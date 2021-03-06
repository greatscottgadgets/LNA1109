# LNA1109

LNA1109 is an in-line SMA Low Noise Amplifier with SAW filter.

## hardware notes

Schematic and layout files were designed in KiCad, an open source electronic
design automation package.

This design may be assembled with any SAW filter with a standard 1.1 x 0.9 mm
footprint.

The PCB is designed to fit the Crystek SMA-KIT-1.5MF housing.

```
order of copper layers:
    Copper 1:  F (front)
    Copper 2:  In1
    Copper 3:  In2
    Copper 4:  B (back)

PCB description: 4 layer PCB 0.8 mm
    Copper       1:  0.035 mm (1 oz)
    Dielectric 1-2:  0.2 mm prepreg
    Copper       2:  0.0175 mm (0.5 oz)
    Dielectric 2-3:  0.265 mm core
    Copper       3:  0.0175 mm (0.5 oz)
    Dielectric 3-4:  0.2 mm prepreg
    Copper       4:  0.035 mm (1 oz)

7628 prepreg with Er=4.6
double side solder mask green
double side silkscreen white
7 mil minimum trace width
5 mil minimum isolation
```

PCBs of this specification are available from JLCPCB (JLC7628 4-layer 0.8 mm stackup).

## frequency options

LNA1109 may be populated with different components to support various frequency
bands.

frequency band | U4 part number       | L1-L4 part number | C1-C6 part number
---------------|----------------------|-------------------|-------------------
902-928 MHz    | FAR-F5QA-915M00-M2AK | HK1005R10J-T      | GCM1555C1H470JA16D
1559-1606 MHz  | F6QA1G582H2JM        | HK100539NJ-T      | GCM1555C1H180JA16D
2402-2483 MHz  | F6FC2G441H4PE        | HK100527NJ-T      | GCM1555C1H100JA16D
