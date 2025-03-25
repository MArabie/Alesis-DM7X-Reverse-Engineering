# Alesis-DM7X-Reverse-Engineering
Reverse Engineering and Pinout to max out the DM7X Module

## Stock Hardware Overview
There is a 25 pin D-Sub connector on the back of the unit:
<br/><img src=https://github.com/user-attachments/assets/ecfdb0f2-f850-4ede-b8ca-a5dc0b9e4b50 height="400"><img src=https://github.com/user-attachments/assets/8719e0bc-bc52-493e-99a3-7168ccdaa281 height="400">
<br/>The cable snake breaks out the drum/cymbol/pedal with just enought cable to reach each when assembled.
<br/>On the Nitro Mesh Kit, there are 3 types terminating connectors:
- 1/4" TRS (Snare, Tom 1, Tom 2, Tom 3, Crash 1, Ride)
    - Snare is a Dual Zone (Drum Pad and Rim)
    - Crash 1 is Dual Zone (Pad w/ Choke)
    - All other are Single Zone
- 1/4" TS (Hi-Hat, Kick)
- 1/8" TRS (Hi-Hat Control)

In addition there are (2) 1/4" TRS jacks on the top of the unit (Tom 4, Crash 2:
<br/><img src=https://github.com/user-attachments/assets/3f7945b8-cc3a-4925-836b-6707d0e3b491 width="750">

## Expansion Pack
Expansion Kit for Nitro Mesh E-drum Set comes with 8" Dual Zone Drum Pad, 10" Cymbal Pad w/ Choke, Mounting Hardware, and 2x 6.25" TRS Cables

## Expandability
Taking the Snare pad from the kit and plugging in the cable for each of the TRS cables, shows each is dual zone (drum or cymbol) capable. The default mapping for drums will be to add a rim sound and for cymbols will be to add a choke. SHoult out to [Bustingsticks with KW](https://youtu.be/MuuOSRGDA14?si=pTXfhj2i3zsDsc4O&t=361) for showing that each Channel can be reprgrammed in the DM7X to a different Voice/MIDI note. So now we can stop thinking about the kit as having 11 cables (9 from the cable snake and 2 from the top of the unit and start thinking about the number of channels. Each TRS cable has 2 channels and the two TS cables has 1 channel.

## Adding on with splitters

## Adding on with breakout
