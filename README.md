# CMC_Lab3_project
## A sound art performance to support Ukraine. 
Catalunya amb Ucraïna. PER LA PAU, LA LLIBERTAT I ELS DRETS HUMANS.
![text](https://github.com/felixCheungcheung/CMC_Lab3_project/blob/main/per_la_pau.jpg)

## Title: “**A Russian Bomber was hit and it crashed finally”**

Introduction: The performance starts with distant explosion sounds together with siren, which means we are facing a war. Then the attention was moved to the bomber, which created the catastrophic soundscape we heard just now. The motion of the mobile phone symbolizes the motion of the flying bomber, meanwhile the tilt and shake movement symbolizes the act of bombing. However, after a loud and clear explosion sound, with special position of the mobile phone, the helicopter sound dims and engine slow down which means it was hit and it finally crashed to the ground.

Technicalities:

Using Puredata, mobmuplat.
Video Demo: https://drive.google.com/file/d/1l1XaKE5P_Bf2odAXbzPXHiUxYLatKeg-/view?usp=sharing

1) Siren : using the GPS **compass** information to control the pitch change, mySlider0 to control its volume;

2) Mapping: 

- **One to many**: X-tilt parameter was mapped not only to control the play back speed and amplitude of helicopter sound, but also the amplitudes of bomb sound which is synthesized using `noise~` , X-tilt also affects band pass filter: changing Q value of (frequency equalization) of bomb sound.

3) **Accelerometer** was used to pass the “shake” information to pd, which would trigger the *plane-crash.wav*

4) **Continuity in timbre**: by moving the phone, the timbre (frequency and volume) of the helicopter sound changes seamlessly, mimicking the flying status; Discontinuity in timbre: explosion sound with different Equalization which indicates different distances of bombed destination.

5) Performed mainly by the motion of the mobile phone rather than moving slides or pressing buttons on the screen.
