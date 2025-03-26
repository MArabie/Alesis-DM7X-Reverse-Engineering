# Alesis-DM7X-Reverse-Engineering
Reverse Engineering and Pinout to max out the DM7X Module

## Stock Hardware Overview
There is a 25 pin D-Sub connector on the back of the unit:
<br/><img src=https://github.com/user-attachments/assets/ecfdb0f2-f850-4ede-b8ca-a5dc0b9e4b50 height="400"><img src=https://github.com/user-attachments/assets/8719e0bc-bc52-493e-99a3-7168ccdaa281 height="400">
<br/>The cable snake breaks out the drum/cymbal/pedal with just enough cable to reach each when assembled.
<br/>On the Nitro Mesh Kit, there are 3 types terminating connectors:
<br/><img src=https://github.com/user-attachments/assets/164556b4-c700-4a55-b2b6-8d4bc51fc64b height="200">![image](https://github.com/user-attachments/assets/705a6643-e459-4c0d-8d96-97e56673deca)


- 1/4" TRS (Snare, Tom 1, Tom 2, Tom 3, Crash 1, Ride)
    - Snare is a Dual Zone (Drum Pad and Rim)
    - Crash 1 is Dual Zone (Pad w/ Choke)
    - All others are Single Zone
- 1/4" TS (Hi-Hat, Kick)
- 1/8" TRS (Hi-Hat Control)

In addition there are (2) 1/4" TRS jacks on the top of the unit (Tom 4, Crash 2):
<br/><img src=https://github.com/user-attachments/assets/3f7945b8-cc3a-4925-836b-6707d0e3b491 width="750">

## Expansion Pack
Expansion Kit for Nitro Mesh E-drum Set comes with 8" Dual Zone Drum Pad, 10" Cymbal Pad w/ Choke, Mounting Hardware, and 2x 1/4" TRS Cables

## Expandability
Taking the Snare pad from the kit and plugging in the cable for each of the TRS cables, shows each is dual zone (drum or cymbal) capable. The default mapping for drums will be to add a rim sound and for cymbals will be to add a choke. Shout out to [Bustingsticks with KW](https://youtu.be/MuuOSRGDA14?si=pTXfhj2i3zsDsc4O&t=361) for showing that each Channel can be reprgrammed in the DM7X to a different Voice/MIDI note. So now we can stop thinking about the kit as having 11 trigger inputs (9-trigger snake cable inputs and 2 from the top of the unit)  as  the manual states and start thinking about the number of channels. Each TRS cable has 2 channels and the two TS cables have 1 channel.  It is not likley the Hi-Hat Control channels can be split, which is probably why they used a 1/8" TRS.

## Adding on with splitters
With the right adapter, 1/4" Female TRS to Dual  14/" Male TS splitter, and a Female to Male (TRS or TS) extension, it is possible to split Tom 1, Tom 2, Tom 3 and Ride from the original kit. You can split Tom 4 and Crash 2 as well depending on if you get the expansion kit or loose parts (ebay).
<br/><img src=https://github.com/user-attachments/assets/4b1b5814-6264-4fb9-a2b2-d2c6731e5290 height="200"><img src=https://github.com/user-attachments/assets/fb0886e7-4e01-49f7-895b-7eac92d10013 height="200">

## Adding on with breakout
DSub 25 break out board and TRS patch cable (TRS on both ends) (get then twice as long as you need them and cut them in half) will also work. This will be more wire in the long run, but will allow more flexibility. Splitters may still be needed for Tom 4 and Crash 2.
<br/><img src=https://github.com/user-attachments/assets/66818b64-ef32-4f4c-856e-80efbd14c66b width="200">
<br/>The pinout for the connector is as follows, from the perspective of looking at the male pins of the connector.
<br/><img src=https://github.com/user-attachments/assets/57d3505f-e47b-43d2-bb03-1ad70dc58183 width="750">
<br/> Table in order of distance from the DSub connector
| Trigger lable on snake connector | Length (inches) | Symbol in diagram | Sleeve(S) Ring(R) Tip(T) | Pin |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| snare | 22 | SD | S | 21 | 
|  |  |  | R | 8 |
|  |  |  | T | 9 |
| hi-hat | 22 | HH | S | 11 |
|  |  |  | T | 24 |
| tom 1 | 33.5 | T1 | S | 19 | 
|  |  |  | R | 7 |
|  |  |  | T | 20 |
| tom 2 | 46 | T2 | S | 18 | 
|  |  |  | R | 5 |
|  |  |  | T | 6 |
| crash 1 | 46 | C1 | S | 22 | 
|  |  |  | R | 10 |
|  |  |  | T | 23 |
| hi-hat control | 54 | HC | S | 25 | 
|  |  |  | R | 12 |
|  |  |  | T | 13 |
| tom 3 | 62 | T3 | S | 17 | 
|  |  |  | R | 16 |
|  |  |  | T | 4 |
| kick | 69.5 | K | S | 15 | 
|  |  |  | T | 3 |
| ride | 73.5 | RC | S | 14 | 
|  |  |  | R | 1 |
|  |  |  | T | 2 |

## Reference Material
https://www.alesis.com/rscdn/1886/documents/Nitro%20Drum%20Module%20-%20User%20Guide%20-%20v1.2.pdf
