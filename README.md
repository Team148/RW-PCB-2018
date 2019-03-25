# RW-PCB-2018


These PCBs are Robowrangler versions of the Talon SRX Breakout Board and a simple CAN Bus Daisy Chain Board. This is standardized around the Molex SL latching type of connector (50-57-9405 + 16-02-0087). This type of connector also connects to US Digital S5 Encoders with the same pinout pattern.

```
Talon SRX Breakout Board BOM
  Harwin M50-3000745     Qty 1 (Cut off outer 4 pins)
  Molex 15-91-3053       Qty 1
  Lite-On LTST-C150KGKT  Qty 1 (Optional)
  Susumu RG3216P-2201-D-T5   Qty 1 (Optional)
  
Based on MVRT / FRC Team 115's Open Source Design.
```

CAN Devices need to be wired into a Molex SL type connectors(50-579404 + 16-02-0087) with the H (green) paired in the middle 2 positions,
and the L's on the outer two positions. The twisted pairs need to be next to each other. Devices must be plugged
in Sequentially and the last device must be terminated with an 120 Ohm resistor (can be PDP). These boards can also
be daisy chained if above 18 devices, simply attach port 15 to another board's port 0.The port numbers are just for reference,
they do not have to correspond to CAN ID.
```
RW CAN
  Molex 70555-0038       Qty 18
```

GERBER Files are exported for SEEEDSTUDIO's FUSION Service


Optional: We recommend using the Belden 8723 060100 wire for encoders and for extending a CAN bus to/from since it both twisted pairs are individually shielded.
