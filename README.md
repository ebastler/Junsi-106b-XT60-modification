# Junsi-106b-XT60-modification
This repository contains all necessary 3D models as well as a short build log explaining how to convert a Junsi iCharger 106b+ to XT60 as input and output connectors. All 3D files will shortly be available at my thingiverse account, too: https://www.thingiverse.com/thing:3005801

![finished chargers](https://raw.githubusercontent.com/ebastler/Junsi-106b-XT60-modification/master/Documentation/junsi_finished.jpg)

### Needed parts
- 2 XT60 (male)
- 20-30cm of 2.5mm² (14 AWG) wire. The more flexible, the better.
- 1 0603 or similar size 100nF 25V SMD cap (not always necessary, but probably)
- 1 non-SMD 1µF 100V ceramics cap with a pin spacing of 8-12mm (only necessary if you work sloppy like me) or 0603 100V caps that add up to 1µF (I used 10 100nF 100V)
- The two 3D printed parts (should be temperature resistant, print in ABS, Greentec or some other filament that endures higher temperatures than PLA)

### Buildlog / Howto
First, open the icharger:
![opened icharger](https://raw.githubusercontent.com/ebastler/Junsi-106b-XT60-modification/master/Documentation/junsi_whole_before.jpg)

You have to de-solder both output terminals (requires a soldering iron with some power. A TS100 powered with 19V does this easily) as well as both input wires. You will probably break the cap right in between the input wires, that's why I recommended having a 100nF 25V ceramic cap at hand. The value is just guessed, but it works and should not be critical as it only is an input buffer. Also, desolder the cap between the output terminals. If possible without breaking it. Mine broke, so I replaced it with 10 single 100nF 100V smd ceramic caps. Use whatever you have at hand as long as it is rated 50V or above and a ceramic cap with 1µF. The value should be a little bit more critical here, seen that it is at the output of the charger.

Then, screw the output 3D bracket in place and insert the output XT60. It should slide in with little force. If it does not, heat up the 3D printed part until it does. Then use a piece of the 2.5mm² wire to solder it to the PCB. Use a lot of solder - these wires will have to mechanically hold the XT60 in place!
![output, work in progress](https://raw.githubusercontent.com/ebastler/Junsi-106b-XT60-modification/master/Documentation/junsi_out_half.jpg)
![output, finished](https://raw.githubusercontent.com/ebastler/Junsi-106b-XT60-modification/master/Documentation/junsi_out_finished.jpg)

If you managed to salvage the cap, solder it onto the two PCB terminals where you connected the XT60 or directly to the connector. Below the connector you can see my SMD cap array ;)

Next, screw the input side cap in place and slide an XT60 in. Again, it should fit with little force. Then connect the negative terminal of the XT60 to the negative pad on the PCB which is located right below. Watch out not to short any of the pads nearby.
![input, work in progress](https://raw.githubusercontent.com/ebastler/Junsi-106b-XT60-modification/master/Documentation/junsi_in_half.jpg)

Now connect the positive terminal of the XT60 to the remaining input pad (again, watch out not to short anything). Your charger should now look somewhat similar to this:
![whole charger, finished](https://raw.githubusercontent.com/ebastler/Junsi-106b-XT60-modification/master/Documentation/junsi_whole_finished.jpg)

All that remains now is closing the charger and enjoy the adpater-free charging!
