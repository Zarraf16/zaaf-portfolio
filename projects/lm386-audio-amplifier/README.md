# LM386 Audio Amplifier

## 🔧 Overview
This project demonstrates the design and implementation of a mono audio amplifier using the LM386 IC. It was built to amplify audio signals from sources like mobile phones or microphones and output the sound through a speaker. The gain is set to the default 20x, and the circuit is built on a PCB designed using EasyEDA.

## 🧰 Components Used
- LM386D Audio Amplifier IC
- Capacitors: 100nF, 100uF (x2), 1000uF
- Resistor: 10kΩ
- Speaker: 4Ω, 10W
- 9V DC battery & cap
- Headphone jack
- IC base
- PCB board
- Multimeter
- Soldering rod

## 📐 Design Details
- **Audio Input**: Supplied to Pin 3 (+Input) with a 10kΩ pull-down resistor to avoid hum when disconnected.
- **Gain Control**: Pins 1 and 8 left open to maintain default 20x gain.
- **Bypass Capacitor**: 100uF capacitor between pin 7 and GND to filter supply noise.
- **Output Path**: Pin 5 connects to the speaker via filtering capacitors (100nF + 1000uF) to handle both high- and low-frequency noise.
- **Power Filtering**: 100uF decoupling cap across power input (Pin 6 to GND).
- **PCB Design**: Done using EasyEDA and adapted slightly during actual implementation for simplicity.

## 💡 What It Does
- Amplifies low-level audio signals from phones or other sources.
- Drives a small speaker with adequate gain and clarity.
- Can be adapted into stereo systems with two amplifiers.

## 🛠️ Challenges Faced
- **Noise Issues**: Minor buzzing at higher volumes due to component quality or soldering.
- **Tools**: Lack of an oscilloscope made signal verification difficult.
- **Solution**: Used IC base to prevent damage, and acknowledged need for better soldering and cleaner power sources.

## 🔬 What I Learned
- How to use op-amp-based audio amplifier ICs.
- Importance of filtering caps in analog circuits.
- PCB layout basics with EasyEDA.
- Real-world issues with noise, grounding, and soldering.

## 📷 Visuals
You can also upload and include circuit diagrams, photos, or EasyEDA schematics here.

## 📄 Full Project Report
[LM386 audio amplifier.pdf](./LM386%20audio%20amplifier.pdf)

## 🔗 Reference
- [Tales From the Chip – LM386 Audio Amplifier](https://www.instructables.com/Tales-From-the-Chip-LM386-Audio-Amplifier)
