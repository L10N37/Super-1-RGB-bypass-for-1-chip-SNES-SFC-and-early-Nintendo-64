<p align="center">
  <img src=Photos/V2.png>
</p>


# Super-1-RGB-bypass-for-1-chip-SNES-SFC-and-early-Nintendo-64

An RGB bypass board for 1-chip SNES/ SFC consoles (Phat & JR). Corrects brightness and wash out issues, same board/ components for both PHAT / JR, attenuated to 0.7vpp output (correct video standards). Uses an LT6550 driver.
RGB may be used to encode the other signals (composite/ S video)
hence, the install methods may kill these outputs. Leaving the factory coupling caps in place will retain the outputs.

Also suits early Nintendo 64 revisions ('easy RGB moddable' revisions such as NUS-CPU-01, NUS-CPU-02, NUS-CPU-03, NUS-CPU-04 and some PAL ones - please check first!), just omit the input attenuation resistors and leave them unpopulated for use in N64!



Update for people using DeJitter mod:

The first kit went out to a gamer who is super happy with his 1-chip :)
He ended up bringing up the fact that

A: He lost the sync attenuating resistor

B: He's using a dejitter mod and used a 75r resistor for sync attenuation

Now, I haven't had any issues with sync on NTSC SFC via OSSC for some reason, but i quickly calculated that you'd want about a 180r to 200r resistor inline from the
dejitter sync out, across to the Super-1 Sync pad. This will give you ~700mV peak to peak which is inline with 75r C sync. 200r calculates to 0.682v and 180 to 0.735v.
Keep in mind we are reducing a 2.5v peak to peak load here and not a full 5v TTL. I'd suggest throwing one in heatshrink with wire each end forming a nice, neat inline resistor wire length. This only applies to straight through TTL C sync cable/ Sync over composite cable. You would jump J1 as well, and if using or planning to use Sync-Over-Composite SCART cable and have disabled composite output, also jump J2.

My twitter is @vajskid ...if you really get stuck.

Note: the guides don't cover sync on luma which is option if you are using phat 1-chip models.
In this case, you can completely ignore the sync jumpers (leave them open) and not install the sync attenuation resistor.



Some results with a cheap unshielded RGB cable, jumpered to route 75r C sync down the composite video line with the onboard attenuation resistor (often this is found in the cable). More photos can be found in the photo folder.

<p align="center">
  <img src=Photos/20220622_121838.jpg>
</p>

<p align="center">
  <img src=Photos/20220622_120940.jpg>
</p>

<p align="center">
  <img src=Photos/20220622_121721.jpg>
</p>

<p align="center">
  <img src=Photos/20220621_193000.jpg>
</p>
