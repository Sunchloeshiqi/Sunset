# Sunset
This is a song that describes the feeling of watching the sunset after school with friends

# Overview
Sunset After School is an original coded music composition created in TunePad.  
The piece captures the warm and cheerful feeling of walking home after school in the sunset.  
It combines multiple instruments — Bass, Drums, Guitar, and Keys. To form a 224-beat structure that slowly builds emotion and ends softly.  
The project was part of the Digital Making Assignment 2 at UTS, focusing on developing code literacy through creative expression.


# Project Goals
- Explore how code can express rhythm and emotion through loops, structure, and timing.  
- Learn to use variables and loops to simplify musical logic.  
- Understand how structure can create emotional storytelling in sound.  
- Apply theoretical ideas from van Dijck (2014) and Kuniavsky (2008) about data and interaction to creative coding practice.  

---

# Features
# Multi-instrument structure
The music consists of four core layers written in TunePad:
- Keys: main chord progression and harmony base.  
- Guitar: rhythmic arpeggios that repeat with variations.  
- Bass: root and fifth pattern creating foundation and pulse.  
- Drums: dynamic rhythm to maintain energy and flow.  

# Loops & Structure
- Used `for i in range(4):` to automatically loop the chord sequence C–Am–F–G.  
- Total duration: 224 beats (all tracks aligned to finish together).  
- Some instruments (e.g. Bass, Guitar) enter later to create layering and variation.

#Variables
Defined note variables for clarity and reuse: 
C3 = 48
E3 = 52
G3 = 55
A3 = 57
F3 = 53
D3 = 50

This made the code more readable and easier to edit when adjusting harmonies.

# Drums Logic
The drum track was created with loops for kick (36), snare (38), and hi-hat (42):
# From beat 32: main groove begins
for i in range(8):
    playNote(36, beats = 1)   # Kick
    playNote(38, beats = 1)   # Snare
    for j in range(8):
        playNote(42, beats = 0.5)   # Hi-hat

Later sections repeat the groove and gradually add intensity before resting at the end.

# Keys Ending
The final chords (B3–E3–C3) act as a soft closure, representing the fading sunset.
It ends the music gently with no drums — only harmony.

# How to Run
Open TunePad.
Create four tracks — Bass, Drums, Guitar, and Keys.
Copy each section of code from /code/ into the corresponding track.
Set tempo around 90–100 BPM.
Press Run / Play to hear the full piece.
Optionally, adjust beat lengths or note pitches to remix the emotion.

# Project Structure
Sunset-After-School/
│
├── code/
│   ├── bass.py            # Bass rhythm foundation (root + fifth, looped)
│   ├── drums.py           # Kick, snare, and hi-hat structure
│   ├── guitar.py          # Arpeggio pattern and repetition logic
│   └── keys.py            # Main chords and harmonic structure
│
├── assets/
│   ├── Sunset_After_School_Final.mp3   # Final exported song
│   ├── screenshots/
│   │   ├── concept_map.png             # Week 11 concept map
│   │   └── tunepad_interface.png       # Screenshot of TunePad interface
│
├── reflection.pdf                       # 1000-word written reflection
└── README.md                            # Project documentation (this file)

# Learnings & Reflection
Through this project, I learned that coding is not just about logic — it’s a way to express rhythm and emotion.
Using loops and variables made me realise that structure and repetition in code are like beats in music: they create flow, tension, and release.
As Kuniavsky (2008) explains, meaningful digital experiences come from interaction and iteration — testing, listening, and adjusting.
Similarly, van Dijck (2014) notes that data carries cultural and emotional value.
In my case, each rhythm and timing decision was not just technical, but emotional.
Code became my way of telling a story through sound.

# References
Cousins, C. (2018, July 18). Vector vs. Raster: What Do I Use? Design Shack. 
  https://designshack.net/articles/layouts/vector-vs-raster-what-do-i-use
Kuniavsky, M. (2008). User experience design for ubiquitous computing. Interactions, 15(6), 20–22. https://doi.org/10.1145/1409040.1409045
Mittelstadt, B. D., Allo, P., Taddeo, M., Wachter, S., & Floridi, L. (2016). The ethics of algorithms:  Mapping the debate. Big Data &        Society, 3(2), 2053951716679679. https://doi.org/10.1177/2053951716679679
Mitchell, M. (2019). Artificial intelligence: A guide for thinking humans. Macmillan.
Van Dijck, J. (2014). Datafication, dataism and dataveillance: Big Data between scientific paradigm and ideology. Surveillance & Society,     12(2), 197–208. https://doi.org/10.24908/ss.v12i2.4776

# Credits
Author: Shiqi Sun
Student ID: 14604894
Course: Working with Data and Code - Assignment 2
University: University of Technology Sydney (UTS)
Platform: TunePad

