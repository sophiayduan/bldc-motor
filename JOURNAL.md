---
title: "A BLDC"
author: "Sophia"
description: "A brushless dc motor"
created: "2025-06-13"
---

Total time: 6.5h


# July 30th: Quick project

**Total time spent: 0.5h**

Planning: 
I'll be using 9 slots / 16 poles, it'll be a pain to wind by hand but I'm trying to have decent torque and rpm at the same time.
The shaft will be held by a set screw, and all the 3D printed parts will be press fit.

<img width="685" height="770" alt="image" src="https://github.com/user-attachments/assets/fb66c80f-7ec0-464f-81ff-29d22a7549cb" />
I also referenced my first 3d printed bldc, it had many many flaws I hope to fix with this design:
- Non existant pressfit
- Shaft is held by friction
- Large for no reason
- Poor CAD
- Circular magnets

# July 31st: Finished
**Total time spent: 6h**
I ended up switching to 9 slots/ 12 poles for a more convential ratio.

Today I finished CADing the entire project, using M2 threaded insert (same as my other project) and some small ball bearings. 

The hardest part was getting the correct dimensions for my stator teeth and rotor, I need to optimize the gap between the magnets, the rotor/stator air gap, keeping the stator teeth reasonable for me to wind by hand and that parts I could find on aliexpress. 

I think I managed to fix all the issues I wanted to tackle with this design.
<img width="577" height="565" alt="image" src="https://github.com/user-attachments/assets/721fc1ea-6a31-4cff-b9fc-cf09fae441e9" />
<img width="441" height="551" alt="image" src="https://github.com/user-attachments/assets/61d95a72-4fa4-443d-bd83-5a041104fdab" />

# Feb 4th: V2.1 Finished
**Total time spent: TOO much**

(Writing this in retrospect) My Aliexpress parts arrived in Sept/Oct, but I didn't have the time to assemble the motor. Or so I thought, I ended up picking this project back up for a school project, and a lot more iterating was done. 

Key changes/additions:
- No more set screw & threaded insert & d-shaft combo, as friction turned out to be more that strong enough
- Used enameled copper wire, originally I had planned (and bought) just regular copper wire
- Powered by a DIY power supply borrowed from my neighbour (had to do some more soldering for this, as originally I was just planning to use a 2-3S LiPo)
- Using a Delta winding configuration (bad idea)
- Simplified parts for 3D printing (less supports needed)
- Added openings on the base, so the wires can actually go through!!
- Used an ESP32 + pot for a servo tester
- Screw holes for mounting
- 3.5mm male banana plugs


This motor did end up spinning, but due to the heat produced by the coils (which was augmented by the delta config), the PLA printed stator started to warp (and melt a bit). This was a huge thing that I missed earlier on, PLA can only go up to 60C approx.

For the next (and likely final) version, i'll swap to Nylon or another high temp filament for the stator, wind it in a Wye (Star) config, and hopefully drive it using a driver board that I design.


Got my hands on a ESC (though I'm designing my own rn)

