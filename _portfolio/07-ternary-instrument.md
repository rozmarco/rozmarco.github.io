---
title: "Ternary-Encoded Dual-Key Musical Instrument"
excerpt: "1st place, IEEE Solid-State Circuits Society Arduino Contest 2023 (Undergraduate). A two-key Arduino instrument that plays melodies by encoding each note as two base-3 digits read from a light sensor."
collection: portfolio
header:
  teaser: ternary/ternary-teaser.png
---

**Problem:** A conventional keyboard needs one key per note. The challenge was to build an 
instrument that can play real melodies with only two keys, using the inexpensive components 
in a standard Arduino kit.

**How it works:** Each note is encoded as two ternary digits (trits). When the player presses the 
note key, a photoresistor reads one of three states: uncovered (0), covered with a white surface 
(1), or covered with a black surface (2). Two presses give 3 × 3 = 9 combinations, each mapped to 
a note, so a binary on/off key would only have given 4. The second key clears a half-entered note 
or pauses playback.

Beyond the core encoding, I added:

- **Pitch bend:** moving a hand toward or away from an ultrasonic sensor bends the current note 
up or down, like a whammy bar
- **Calibration mode:** captures the light reading for each trit and sets the pitch-bend 
range, so the instrument works under different room lighting
- **Note-selection mode:** lets the player assign any of 28 pitches (F♯3 to A5) to the nine trit 
codes, so the instrument can be retuned for each song

I designed the encoding scheme and wrote the firmware in C++ on an Arduino Uno, and annotated 
sheet music in trit notation to play pieces such as Bach's Minuet in G.

**Result:** 1st place, IEEE SSCS Arduino Contest 2023 (Undergraduate category, Music Season), 
which included a $1,000 prize.

[![Demo video](https://img.youtube.com/vi/beMKSZGa-6o/0.jpg)](https://www.youtube.com/watch?v=beMKSZGa-6o)

**[Watch the demo](https://www.youtube.com/watch?v=beMKSZGa-6o)** · 
**[Source code on GitHub](https://github.com/rozmarco/ternary-arduino-instrument)** · 
**[Contest winners page](https://arduino-contest.sscs.ieee.org/winners)**

**Tools:** C++, Arduino Uno, photoresistor, ultrasonic ranging sensor, piezo buzzer, servo