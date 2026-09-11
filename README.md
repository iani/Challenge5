
# Bodily Movement & Sounding Spaces

Movement-driven live sound and optional graphics—your academic challenge.

# Description

**Bodily Movement & Sounding Spaces**: 

Your body becomes an instrument. Create a system where bodily movement becomes part of the music. Movement can control sound and graphics, but it can be more than that. This challenge invites you to explore that connection using AI and sensor technologies to turn movement into a rhythmic, melodic, or expressive layer of the music itself.

Challenge:  
How can a live performer’s movement create sound and graphics in real time for a given topic?

Challenge Questions:

1. How can “Movement” control sound? And can it be more than that?
2. Can you create an interactive environment where the performer’s movements, captured by a standard webcam or a dedicated tracking camera, generate live sound and optionally also graphics in any synthesis or gaming environment?
3. How can you use phones, wearable sensors to capture gesture, rhythm, motion, or physical energy, and map this data to synthesis, VST instruments, samples, existing songs, or any audio recording?

Available Tools: webcams, projection, PA system and rehearsal space. 

Other very welcome tools: Arduino with sensors of all kinds, other sound synthesis software, building custom sound synthesis and graphics from scratch, MediaPipe, gaming engines (Godot, Unity, Unreal engine). 

Starter kit provided: SuperCollider, PureData, Godot Engine, XR-Animator.

# Examples

The following are examples of performances and rehearsals from the proposer of this challenge, Iannis Zannos.  These are art projects in a contemporary/electronic music context.  These examples show how to use movement data to control sound in performances.  You are welcome to develop your own style which can be radically different from that of the examples below.  

Note that the performances were made using wearable sensors which send only a few parameters from hands or legs.   The BuMoChi tools and/or XR-Animator proposed here can get live data from the entire body, including face and fingers.  You are welcome to use any other motion tracking tools of your choice as well. 

## Performances

Izutsu Daphnis Echo Fantasy (Tama Fest, Tokyo 2020)
https://youtu.be/QoFKtLOzpAk?list=PL1yHvCYr9Bvavc0uX4iNi4SdsMx1Y-w_4

Takekurabe (TTT Conference, Malta 2023) Malta-Tokyo
https://youtu.be/Mz2_rH3Cd-4?list=PL1yHvCYr9BvZhTc2lfahAS7as_2abajKc

Takekurabe (Musika Viva Festival 2022.  Lisbon, Portugal and Corfu, Greece).  Remote sound control from Tokyo from motion data sent via OSC. Graphics by openFrameworks. 
End-to-end montage of takes from Corfu and Lisbon
https://youtu.be/xT2nPo8Hfu4?list=PL1yHvCYr9BvZs44mcmGdybH6tPu4aMLp1

Izutsu (Elevsis23 Festival, Elevsis 2023). Major work, story adapted from the Noh play Izutsu. 
https://youtu.be/HXPeVC3PqqM?list=PL1yHvCYr9BvZFqh6kf1flXM-P6x1dr2LM&t=2059
Or skip to the beginning of sensor-driven sound:
https://youtu.be/HXPeVC3PqqM?list=PL1yHvCYr9BvZFqh6kf1flXM-P6x1dr2LM&t=2201

## Rehearsals and Experiments

First experiment with sensor.  Granular Synthesis, 2018.
https://youtu.be/ei-U3KzFCv4?list=PL1yHvCYr9Bvay6kAj6jVNmeD98IFw4kWt
First dance session with wireless sensor

Remote rehearsal Ebetsu (Hokkaido, Japan) - Corfu (Greece) 2020
https://youtu.be/xT2nPo8Hfu4?list=PL1yHvCYr9BvZs44mcmGdybH6tPu4aMLp1&t=53

IDE Fantasy Trailer EASTN DC
https://youtu.be/0GVUBwPKhxY?list=PL1yHvCYr9BvZs44mcmGdybH6tPu4aMLp1

Scene rehearsals for Izutsu 2023
Rehearsal 1
https://youtu.be/O0PrvWVPPps?list=PL1yHvCYr9BvZcRtSh8X4bpELVnQyCXPVs

Chaotic sound algorithms on SuperCollider and graphics on openFrameworks 2022
https://www.youtube.com/watch?v=1UY_kXaMiSg&list=PL1yHvCYr9BvZs44mcmGdybH6tPu4aMLp1&index=3

Chaotic algorithms with multiple parameters. Control and dialogue experiments 
https://youtu.be/S6LJ83-Oomk?list=PL1yHvCYr9BvaRmqKqdk__ikIfC-ovISzY
Chaotic Sound Session 7. Third and final Duo with Jun Takahashi and Asayo Hisai (Tokyo, 2020)

Controlling sound from full-body Mocap with Rokoko suit. First experiments. 
https://youtu.be/6sJYkYKONKo?list=PL1yHvCYr9Bvb-1PIrIZyGlU0EZlpQdjLB
Controlling sound in SuperCollider from live animation data on Godot/Rokoko

(Corfu-Athens, 2025)

# Starter kit: Webcam Motion Capture Software, SuperCollider, Godot. BuMoChi library

The BuMoChi library for live animation and sound synthesis control via webcam is available here: 

https://github.com/iani/bumochi

The BuMoChi library uses XR-Animator, a free tool that works with laptop webcams or any other external webcam for motion capture, and Godot engine, a free gaming engine for animation.  It provides python scripts for converting XR-Animator VMC bundles into single OSC messages.  It also provides Godot projects tuned and tested for working with these OSC messages, and (under development) tools for connecting, recording and configuring the playback of mocap data.  

You can use this library to connect to SuperCollider, but also to any other OSC capable sound making software, such as PD or Max/MSP.  
