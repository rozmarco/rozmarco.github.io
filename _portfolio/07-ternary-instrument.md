---
title: "Ternary-Encoded Dual-Key Musical Instrument"
excerpt: "1st place, IEEE Solid-State Circuits Society Arduino Contest 2023. A two-key instrument capable of playing full melodies using ternary encoding — hardware-software co-design in C++."
collection: portfolio
---

**Problem:** Standard digital instruments map one key to one note. The challenge: design a 
musical instrument using only two buttons that can play full melodies — requiring a richer 
encoding scheme at the hardware-software interface.

**My contribution:** I designed a ternary encoding scheme (base-3 rather than binary) where 
combinations of two-key press states (press, hold, release timing) encode distinct musical 
commands. The instrument uses an ultrasonic sensor for continuous pitch modulation, a 
photoresistor for secondary control, and a servo for physical expression — all orchestrated 
in C++ on Arduino Uno.

**Result:** 1st place, IEEE SSCS Arduino Contest 2023 (Undergraduate category, Music Season). 
The instrument successfully plays multi-note melodies and allows real-time pitch variation 
through physical gesture.

[![Demo Video](https://img.youtube.com/vi/beMKSZGa-6o/0.jpg)](https://www.youtube.com/watch?v=beMKSZGa-6o)  
▶️ [Watch the demo](https://www.youtube.com/watch?v=beMKSZGa-6o)

**[GitHub — Full source code](https://github.com/rozmarco/ternary-arduino-instrument)**

**Tools:** C++, Arduino, ultrasonic sensing, photoresistor, servo control
