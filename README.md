# MaskMoistureMeter

## About this project

A simple device that measures the moisture of face masks. It uses a 555 timer to measure the resistance of cloth.

If the mask is dry, it lights up a green LED. If the mask is moist it blinks a red LED and also beeps with a piezo buzzer.
The faster is blinks and the higher the beepers pitch the more moisture is in your mask.

Replace and/or wash moist masks immediately as wearing a wet mask is dangerous to your health.

The electronics was designed in KiCad and has all information tor order it assembled from JLCPCB.

## Project files

- case: The case as a step and stl file
- fabrication: Gerbers, bom and pick and place files, made according to the JLCPCB free SMT assembly specs
- images: Some images of the PCB, assembled PCB and the case
- pcb: KiCad project files

## PCB specs

- 2 layers FR4
- EIG finish recommended so the sensor area doesn't oxidize
- Board thickness 1mm - otherwise it won't fit the included case

## Parts

### BT1
Battery holder for a CR2032 coin cell. Alternative to LCSC part: Keystone 1060.

### BZ1
The buzzer. Murata PKMCS0909E4000-R1 - can be left out for LED indication only.

### C1 and C2
100nf 0603 capacitor. Use any one with at least 5% tolerance and 6.3V voltage rating.

### D1 and D2
0805 LED in green (D1) and red (D2). Use LEDs with a forward voltage of under 2.8V.

### R1 and R2
0603 resistor with about 150 ohm. Adjust to tune the brightness of your LEDs.

### R3
0603 resistor with 1k.

### SW1
5.1x5.1mm SMD push button with gullwing pins and a height of 3 to 3.5mm.
Alternatives to the LCSC part: Würth 430451035836 or C&K KSC341GLFS

### U1
555 timer IC in 8-SOIC package that works at 2V.
You can use: TLC555CDR, TLC555IDR, TLC555QDR or TLC555CD

## Video Demo

[See it in action here](https://www.youtube.com/watch?v=t6rHHnABoT8)

## Assembled device in case

![Meter in case](https://github.com/RickP/MaskMoistureMeter/blob/master/images/Case_front.jpg?raw=true)
