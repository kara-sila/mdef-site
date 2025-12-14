# Unpacking Tech Systems

## The Machine Paradox

“The Machine Paradox, also known as The Almost Useful Machines (TAUMS), is a project that challenges participants to design and build "useless" machines. These machines are designed to provoke critical thinking about technology and its relationship to society. The paradox lies in using seemingly unproductive creations as tools for exploring complex concepts like technological determinism and the impact of technology on human experience. Through the Machine Paradox, participants engage in hands-on, experimental learning that encourages a more critical and personal approach to technology.”

![GIF_20251120_192716_178 (1)](https://github.com/user-attachments/assets/d48f68d7-edbe-47e4-8f72-362cdefb31c3)

## Hacking the Radio: From Utility to Uselessness

We repurposed a Sunstech vintage radio, completely gutting its internal components and transforming the existing casing into the shell for our device. The opening where the original speaker once was now serves as the stage for our mechanical clown. Inside the box, three gears powered by an Arduino and controlled through a joystick, animate the clown’s pop up experience. When the joystick is pushed upward, the system triggers the clown to spring through the speaker opening and deliver a prerecorded message revealing to all naive children that: “Santa is not real”. Instead of producing meaningful audio, the machine becomes performative, ironic, and self-referential. 

![IMG20251128120859](https://github.com/user-attachments/assets/f2c53a53-e36b-4cc2-8d94-6d09a24db734)

In order to achive this, we first tried to hacked two parts of the radio; the LCD and control module and the speaker.

### Hack #1: The LCD and Control Module
<img width="646" height="484" alt="image" src="https://github.com/user-attachments/assets/3194d793-ae2d-4ada-ada6-2a7663d4cb0a" />

One of the main components we wanted to work with was the control module. It was a circuit board in the front that held a microcontroller, an LCD module, buttons that were activated using silicon buttons with a conductive base, and a variety of smaller components to support these. The board had it's own microcontroller. On further inspection and research, the microcontroller had functions to control the entire device. It had inputs from the buttons and outputs to the components to allow for tuning through FM and AM Oscillators, memory storage and button control to access them (through the numpad), and other such features. We wanted to hack the chip to be able to access these controls but we were not sure of how to go about this.

<img width="1080" height="646" alt="image" src="https://github.com/user-attachments/assets/64667751-09c8-456f-9b6c-33ce87cd47d0" />
We attempted to transform part of the circuit board into capacitative touch sensors to build a digital controller. We repurposed the numpad buttons built-into the right side of the circuit board panel from the radio and connected it to the sensor pins of the Arduino. The original board had 6 buttons on the left that were designed to change radio settings when touched; and 9 buttons on the right in the form of a numpad that were controlling saved radio stations. To interface this with our computer, we soldered wires from the circuit-buttons on the radio’s PCB to the numbered input pins on the Arduino.

You can [click here](https://hackmd.io/@NMSoU2fTSTmrp4ucDbylgw/r1bYmChgbx) for the full hacking report.


### Hack #2: The Speaker
<img width="4032" height="3024" alt="image" src="https://github.com/user-attachments/assets/b8df91ed-97a0-4830-9b1d-fad50bb7371a" />

When we opened up the radio, we found a passive speaker, and a PCB board. Our goal was to tap into the speaker system and create our own external amplifier, controlled by an Arduino. The internal speaker was a simple passive driver, meaning that we needed an amplifier unit. First, we tried to build our own amplifier with LM386 audio amplifier, IC Capacitors (10 µF, 100 µF, 0.1 µF), and a 10k potentiometer.

<img width="1280" height="991" alt="image" src="https://github.com/user-attachments/assets/1633b28d-44f8-4e18-8a95-c2981215b589" />

You can [click here](https://hackmd.io/qp2S-dgZQey9tZz_A9kBEQ) for the full hacking report where tried to build our own amplifier. 

Then, we found the original amplifier on the PCB board under the heatsink and decided to use that instead. First, we tried to record a voice and store it with the original inputs of the radio. However, the memory capacity didn't store even 60KB data. In order to solve this, we decided to use a DFmini Player. 

## The Killjoy

We repurposed the speaker with our own audio using the amplifier of the main board from the radio. We reprogrammed the touch sensors from the original radio buttons to stimulate different sounds. Our main aim was to combine these two hacks to create our own useless mechanism.

We used a Barduino, DFmini player, a speaker and a joystick. We recorded the audio to store inside the DF Player, and controlled the audio using joystick; when the joystick is used the next audio is played.

![IMG_3874 2](https://github.com/user-attachments/assets/08d4d0cd-1e20-405c-8b3f-4fc85cdd7c45)
![circuit](https://github.com/user-attachments/assets/e88bdae8-5d84-4dcf-a451-38c53bb23a6e)

For the mechanism of jack-in-the-box system, we tried different propotoypes first using cardboard, then we laser cut MDF pieces and 3D printed some parts to test the mechanism. 
<img width="779" height="935" alt="1" src="https://github.com/user-attachments/assets/094001f3-5075-4517-af06-7befe658f148" /> <img width="348" height="670" alt="2" src="https://github.com/user-attachments/assets/e7d8fb90-19c6-4de1-a77b-9922c3b562c3" />
<img width="936" height="756" alt="3" src="https://github.com/user-attachments/assets/34594fdb-05a7-441c-86c3-3170edd375ee" /> <img width="938" height="1029" alt="5" src="https://github.com/user-attachments/assets/2ff21477-2467-4a42-a3df-a6bbbdecef83" />
<img width="823" height="1266" alt="6" src="https://github.com/user-attachments/assets/8c03415f-1edc-4dda-aa55-e0117e84305e" />

### The System Diagram
<img width="1003" height="461" alt="Screenshot 2025-12-14 at 16 56 46" src="https://github.com/user-attachments/assets/edac11c9-8ffa-486a-8425-ec2294acd424" />

Full Presentation:
[Group 4_The Radio_Final Presentation.pdf](https://github.com/user-attachments/files/24151367/Group.4_The.Radio_Final.Presentation.pdf)

https://www.youtube.com/watch?v=MOrXRBSLM7c
