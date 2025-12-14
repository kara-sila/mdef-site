# Unpacking Tech Systems

## The Machine Paradox

“The Machine Paradox, also known as The Almost Useful Machines (TAUMS), is a project that challenges participants to design and build "useless" machines. These machines are designed to provoke critical thinking about technology and its relationship to society. The paradox lies in using seemingly unproductive creations as tools for exploring complex concepts like technological determinism and the impact of technology on human experience. Through the Machine Paradox, participants engage in hands-on, experimental learning that encourages a more critical and personal approach to technology.”

![GIF_20251120_192716_178 (1)](https://github.com/user-attachments/assets/d48f68d7-edbe-47e4-8f72-362cdefb31c3)

### Hacking the Radio: From Utility to Uselessness

Our intervention aimed to transform the radio into a jack-in-the-box–like useless machine — a system that activates itself only to negate its own purpose. Instead of producing meaningful audio, the machine becomes performative, ironic, and self-referential. In order to achive this, we hacked two parts of the radio; the LCD Module and the speaker.

## Hack #1: The LCD Module


## Hack #2: The Speaker
<img width="4032" height="3024" alt="image" src="https://github.com/user-attachments/assets/b8df91ed-97a0-4830-9b1d-fad50bb7371a" />

When we opened up the radio, we found a passive speaker, and a PCB board. Our goal was to tap into the speaker system and create our own external amplifier, controlled by an Arduino. The internal speaker was a simple passive driver, meaning that we needed an amplifier unit. First, we tried to build our own amplifier with LM386 audio amplifier, IC Capacitors (10 µF, 100 µF, 0.047 µF), and a 10k potentiometer.
<img width="1280" height="991" alt="image" src="https://github.com/user-attachments/assets/1633b28d-44f8-4e18-8a95-c2981215b589" />
You can [click here](https://hackmd.io/qp2S-dgZQey9tZz_A9kBEQ) for the full hacking report where tried to build our own amplifier. 

Then, we found the original amplifier on the PCB board under the heatsink and decided to use that instead. 
