# Pulse Oximeter Prototype

**Total time:** ~19 hours  
**Duration:** 6 days  
**Start date:** January 12  
**End date:** January 17 

> Research and 3d model were already completed before this journal.  

![1.png](/1.png)
---

## Day 1 – January 12
**Time spent:** ~4 hours

I started the project by working on the electronics design. The main goal for this day was to create a schematic for a standalone ATmega328p instead of using a full Arduino board, mainly to reduce cost and have more control over the system and honestly i said why not.

Using KiCad, I designed the full schematic, including the power section, reset circuit, and the 16 MHz crystal oscillator with its capacitors. I carefully mapped the connections based on the Instructables guide but adapted everything to fit the ATmega328p pinout rather than an Arduino Mega.
![s.jpeg](/s.jpeg)


---

## Day 2 – January 13
**Time spent:** ~2 hours

On the second day, I prepared a list of the compoenents i needed and i went to RAM Electronics to purchase the components, including the LEDs, phototransistor, resistors, capacitors, and the LCD. i already had an atmega328p.

After returning, I organized the components and double checked their values against my schematic to make sure everything matched the design before starting assembly.

![2.jpeg](/2.jpeg)
![3.jpeg](/3.jpeg)

---

## Day 3 – January 14
**Time spent:** ~5 hours

This day was focused on building the main circuit. I followed the general logic of the Instructables project, but with two key changes: I used a standard LCD instead of a TFT screen. I used an arduino uno instead of an Arduino Mega due to budget limitations. I assembled the full circuit on a breadboard, including the microcontroller, LED driving resistors, and the phototransistor configuration. This step took a significant amount of time because I had to carefully verify each connection and ensure compatibility with the modified design. i used ardunio uno instead of the atmega328p chip to reduce the time.

![5.jpeg](/5.jpeg)
![6.jpeg](/6.jpeg)
![7.jpeg](/7.jpeg)

---

## Day 4 – January 15
**Time spent:** ~1 hours

On the fourth day, I worked on the sensor housing. Instead of a 3D-printed enclosure, I used a clothes clip combined with black wrapping material. The black color was essential, as lighter colors interfered with the IR and red LED light paths.

I securely fixed the IR LED, red LED, and phototransistor in proper alignment to ensure accurate readings. After finishing the sensor assembly, I placed it inside a small protective box to reduce the risk of damage or accidental disconnection during testing.

![f.jpeg](/f.jpeg)

---

## Day 5 – January 16
**Time spent:** ~3 hours

 I wrote the code for the Arduino uno, adapting the logic from the original project to work with the arduino and the LCD display.
After uploading the code, I conducted functional testing . The device successfully detected pulse signals, confirming that both the hardware and software were working as intended.

![c.png](/c.png)

## Day 6 – January 17
**Time spent:** ~4 hours

In the final day I transitioned away from using the Arduino Uno and built a standalone ATmega328P circuit instead. After burning the bootloader and verifying stable operation, I transferred all connections from the Arduino Uno to the ATmega chip. This step reduced the overall size of the system and made the circuit closer to a final, independent design. Extra care was taken to recheck pin mappings and signal integrity to ensure the circuit functioned identically to the Arduino-based setup. then i recorded a test plan video to demonstrate the system’s operation.

![ff.jpeg](/ff.jpeg)