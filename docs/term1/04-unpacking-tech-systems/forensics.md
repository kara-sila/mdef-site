# Unpacking Tech Systems

## Forensics of Obsolescence

In this course we approached machines not as neutral tools, but as artifacts embedded in systems of production, use, neglect, and abandonment. Through forensic analysis, dismantling, and speculative reconfiguration, we examined how everyday technologies fail, not necessarily because they stop functioning, but because they lose relevance within shifting socio-technical conditions.

The central question was not how to fix machines, but how to understand them; which part is used for which function, has it opened and hacked before, and how can we use its parts to create something without the limits of keeping everything functional, efective or useful.

You can read the full forensic report by [clicking here](https://hackmd.io/VbZAbcETQPGsrWOHqo6woQ).

### The Radio
The chosen object was a Sunstech Arch Audio RP-RD3000, a retro-style AM/FM radio designed for domestic use. At the time of examination, the device was somehow operational. Its status was not broken, but obsolete.

![IMG_5544 (2) copy](https://github.com/user-attachments/assets/98693265-5138-4d1b-bb08-ea8b27fe4163)


#### The Analysis
We conducted a full forensic teardown of the radio, treating it as evidence rather than equipment. The process included:
- External and internal disassembly
- Component cataloguing and documentation
- Material and manufacturing analysis
- Power and signal testing using lab equipment
- Functional tracing of signal flow and control logic

All components were laid out, identified, and documented individually to expose the internal logic of the machine. We also recorded every step of the process to make sure that we would be able to reconstruct everything back.

The radio operates as a hybrid system: analog signal processing (AM/FM reception and demodulation), digital user interface (LCD display, button controls, presets), transformer-based power supply, internal passive speaker with amplification stage.

##### Radio Mode
Radio Waves → Antenna → Tuner → Demodulator → Audio Amplifier → Speaker → Sound
Microcontroller → LCD + Buttons

##### AUX Mode
External Device → AUX Input → Audio Amplifier → Speaker → Sound

<br>
#### A Twist!
There was also something really interesting about the radio, which made us intrigued! When we opened up the readio, we realized there's one part that looks like it was added later the production since it looked like a delicate connection which is prone to bozulma incase of a crash or drop. Later we realized this part is the antenna of the radio; several yarn strings attached to an cylindirical object. After examining the structure we realized it might be how the radio is produced during the manufacture process, and if that's the case, this is a clear example of planned obsolesence!

![IMG_3668 2 (1)](https://github.com/user-attachments/assets/5f45e519-aa76-4e9a-a70f-68ad68224d51)


