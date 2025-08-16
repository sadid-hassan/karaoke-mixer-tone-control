# karaoke-mixer-tone-control
A 5-block audio system implementing **mixer/karaoke**, **Baxandall tone control** (bass/treble), **volume**, **LED volume display**, and **output attenuation/buffer**, designed, simulated (Multisim), and implemented on breadboard and PCB.

**Highlights**
- Mixer/Karaoke: SPDT-selectable **inverting summer** and **subtracting amplifier** (–(L+R) vs. L–R).
- Baxandall tone control: bass/treble boost/attenuation using RC networks and op-amp stages.
- Volume: potentiometer divider with predictable max/min levels.
- LED Volume Display: 4 comparators with resistor ladder thresholds (0.25V, 0.5V, 1.0V, 1.5V).
- Output Attenuator/Buffer: inverting op-amp sized to drive headphones safely (≈0.5–1.0 V). 
