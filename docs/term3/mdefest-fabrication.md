# MDEFest Fabrication

<img width="684" height="581" alt="Screenshot 2026-06-19 at 18 11 13" src="https://github.com/user-attachments/assets/e41ae13a-e482-4a67-be67-5b5a741c08e4" />

## [Project Website: https://kara-sila.github.io/affective-ruptures/](https://kara-sila.github.io/affective-ruptures/)


## Affective Ruptures: Reclaiming Joy in Public Space
This research began with a simple question: how can we trigger bizzare behaviours in public spaces where it is not expected or allowed. The main idea is that triggering bizzare behaviors through sensory devices and somatic practices will allow us to reclaim our presence and use joy as a political act. The initial impulse was to make that invisible threshold tangible, not through representation but through direct somatic experience. The wearable module became the material answer to that question together with the card deck.
The first technical challenge was more basic than expected. Getting a vibration motor to respond to an ultrasonic sensor took longer than anticipated, mostly because the hardware debugging process revealed how much can go wrong between a circuit diagram and a breadboard. Transistor orientation, wire contact quality (especially on LEDs).

https://github.com/user-attachments/assets/aacd1856-0c63-4488-b04d-efaeca0e4452

The architecture evolved from a single-unit prototype (XIAO ESP32-S3 + Grove Ultrasonic Ranger + ERM motor) into a two-unit wireless system using ESP-NOW. This shift was significant both technically and conceptually. I started with single-unit to test the concept in a public space as a auto-etnographic research, and then moved to two-unit structure. Separating the sensing unit from the haptic unit meant the body could carry two discrete modules: one that reads space, one that responds to it. Also it allowed me to test both units on two different bodies, in that scenario one body was creating the trigger and the other was receiving the feedback. In both trials bodies become part of the circuit.

ESP-NOW proved to be the right protocol for this, low latency, no router dependency, peer-to-peer. The debugging process around MAC addresses, port confusion between two simultaneous XIAO units, and callback signature changes in newer ESP32 library versions was slightly difficult.
Adding another control to the motor with analogWrite allowed the vibration intensity to scale smoothly with distance, which changed the feel of the interaction entirely. A binary on/off trigger produces a startle. A gradient produces something closer to pressure.

<img width="480" height="640" alt="IMG_7532" src="https://github.com/user-attachments/assets/38fe1715-2cfe-426b-bf3d-3d6f372ebc13" />

The NeoPixel LED strip introduced another sensory layer. The color logic, green at distance fading through blue and purple into red as proximity increases, maps the same gradient the motor expresses but makes it visible rather than felt. The LED strip also revealed how much small hardware details matter: incorrect end connection, wrong pin selection. Each of these required diagnosis and correction. But at the end having an LED strip helped me amplify the feedback of the trigger both for the feeling body and for the audience as well. 

<img width="480" height="640" alt="IMG_7546" src="https://github.com/user-attachments/assets/935ed71b-c06d-427e-a8fe-55bdd5d7bbb9" />

After figuring out the inputs and outputs i was designing the closing as a 3D printed structure; however, while thinking about the function of the artifact, i wanted it to act as a second skin. That's why I used silicon (color code: flesh) to create a skin-like but shiny layer. 
At this point I experimented with conductive tape and conductive thread to use silicon just like a textile. However tape doesn't stick to silicon and thread was also not suitable for the almost flesh-like quality of the silicon. 
<img width="480" height="640" alt="IMG_7482" src="https://github.com/user-attachments/assets/00651919-dcac-426b-9b2f-3e1d1459c0fb" />
<img width="480" height="640" alt="IMG_7457" src="https://github.com/user-attachments/assets/63935b82-a3f0-437b-bc28-aac221a00f02" />


At the end I removed the breadboard and used perforated board to make my electronical part as thin as possible. I experimented with different thicknesses of the silicon to try on skin; a thicker layer allowed me to stitch the electronics and thin layer of silicon was better to use it as an outer layer that it's easily sticking itself.
<img width="480" height="640" alt="IMG_7459" src="https://github.com/user-attachments/assets/425170b3-21e1-4822-8652-c3ca3917197a" />



### Theoretical grounding
<img width="480" height="640" alt="IMG_7501" src="https://github.com/user-attachments/assets/26038e65-7a31-4035-b451-7ebc251a32d4" />

The project sits within a broader inquiry into bodily autonomy and spatial politics in public transit corridors, developed through the Affective Ruptures research. Drawing on Kristina Hook's somaesthetics, the design takes seriously the idea that the body is a site of knowing, not just a vessel that carries a mind through space. The vibration is not a notification. It is an interruption, a rupture in the trained compliance that public spaces produce.
Audre Lorde's writing on the uses of the erotic, and Adrienne Maree Brown's emergent strategy framework, both suggest that pleasure and sensation are not secondary to political life but constitutive of it. A wearable that continuously monitors and responds to proximity asks the wearer to remain attentive to their own boundaries, not as a cognitive act but as a felt, ongoing experience.

Also, another part of the project was the Card Deck which was used within the protocol of the performance, especially during the workshop. For the full Card deck you can check this pdf:
[Card Deck.pdf](https://github.com/user-attachments/files/29216604/Card.Deck.pdf)

These were the initial visuals created for the cards by yours truly;
<img width="1668" height="2388" alt="Untitled_Artwork" src="https://github.com/user-attachments/assets/c9ce540f-5f6f-4d9b-98cc-c69333bbc1c8" />
<img width="1668" height="2388" alt="Untitled_Artwork 3" src="https://github.com/user-attachments/assets/0a2d1784-fb06-4291-85df-e3b2f24e2cbc" />
<img width="1668" height="2388" alt="Untitled_Artwork 2" src="https://github.com/user-attachments/assets/99b8a570-a193-4b79-8425-1749abc1dc78" />


## "We cannot build a better world from a place of numbness and deprivation. We need to practice feeling good as part of how we get free."
Adrienne Maree Brown, Pleasure Activism, 2019

<img width="640" height="480" alt="IMG_7549" src="https://github.com/user-attachments/assets/b63622c6-fb94-4b84-a436-72da3e68869e" />

### Cognitive Contribution Label (CCL)
<img width="1200" height="560" alt="CCL_Affective_Ruptures_Sıla" src="https://github.com/user-attachments/assets/65f8b271-302e-4532-8938-5eecddf74680" />

