# Tarmo 4 HP V2.1

### Tarmo 4 high performance V2.1

### DISCLAIMER

This project is a derivative work based on Tarmo 4 and Tarmo 5, 
originally released under CC BY-NC-SA.

Modifications include:
- Reinforced chassis
- Updated suspension geometry
- High-performance drivetrain configuration
- Much more

Please visit the Links section at the end for links to Tarmo 4 and Tarmo 5. 

This project is not affiliated with or endorsed by the original creator.

⚠️ **Project Status: Work-in-Progress**  
This is a high-performance RC car that works, but has known issues (see below).
**Print at your own risk** — some parts may require iteration.

### Purpose: 

To test out the limit of 3D printed RC cars and to design a high performance version of the Tarmo chassis. 

### Changes:

1. **Stronger motor** I replaced the original motor (a D3542) with a high power hobbywing 4274 that can do 150A at 6S. This not only allows the car to be able to go faster but it opens a whole range of other possibilities for other motors eg. sensored setups for better torque and acceleration or even a dual motor setup. It also comes with its own adaptor and mount. 
2. **Enlarged chassis** With a larger power system and drivetrain comes a longer chassis. The chassis length has increased from 359mm to 470mm and the width has also been increased to roughly the same as the original suspention. 
3. **Remade shafts** The driveshafts are now much thicker and can be printed horizontally, meaning that it does not have to be printed out of TPU again. Everything now uses 15x24x5 bearings which not only increases the overall strength of the setup but also makes sourcing parts less complicated. The gears are also partly redesigned to allow it to fit with the new shafts. Furthermore this also eliminates the weak point that is the input gear for the diffs.
4. **Gear ratio change** The overall gear ratio has been changed to 1:2 because i made the central gears 1:1. I made this change to allow for higher speeds because a 4274 should have no problem pulling the car with is being quite light (2-3kg lighter than a Arrma limitless i believe).
5. **Gear changes** I also changed the middle gears since in testing they kept stripping hence i increased their modulus. I also increased tolerances so that the entire drivetrain spins much smoother. 
6. **Changes specifically for 3D printing** Most of the parts on the car can now be printed with no supports (or with easy to remove sacraficial supports) except for the central gearbox lid (minimal supports), the rear diffs, the front suspention mount and the driveshafts. Even those that do require supports require only a small amount (except for the driveshafts and the rear diffs) and can easily be removed by hand. I am currently working on removing them or designing small sacraficial supports directly into the model. 
7. **CV joints** I copied the Tarmo 5 CV joints over and slapped them on it since i believe they are designed beautifully and it would be a shame not to put them on. It also solves the reliability issue of dogbones that i was experiencing during previous testing. I also changed out the shaft in the middle of the Tarmo 5 Cvs with my own beefier design. I then thickened the CVs to about twice the thickness to increase strength and standardise the bearings so that only one type of bearing is needed throughout. The CVs even though after the change are still too thin and broke once after I tried to do a very fast drift. 
8. **Suspension changes** I thickened the kunckles to accomodate larger CVs and also to strengthen the entire thing after several failures of the CV joints.
9. **Bar in the middle** There is now a detachable bar in the middle in order to make the car chassis stiffer. I originally made it so that it is one part with the central gearbox lid but then changed it so that it is detachable that way iteration is easier.
10. **Others** Integrated gopro mount, integrated batter mount, integrated ESC mount (not taped on anymore!), proper steering links (not 3D printed), redesigned front wheel mounts (easier to print and more reliable), a bar to make the chassis stiffer, a dedicated wheel mounting thing for Arrma Dboot tyres and so much more.

For more information on specific changes and how the design evolved over time, see the changes section. 

### How can you build one? 

Here are 5 easy, no-nonsense steps that you can follow to build it. If you follow the steps carefully it should be quite easy to build (i spent so much effort on making sure that the tolerances are right and to simplify the build process). 

##### Step 1: Make sure you own a 3D printer with the right specs
- minimal 256x256x100mm build area (standard bambu lab size)
- can do nylons (~280 nozzle, ~100 bed, ideally enclosed)
- calibrated (important, make sure to do flow calibration as well to make sure tolerances are all right)
- can do CF and GF filled abrasives (hardened steel / gemstone nozzle) (i have a hardened steel one and a obxidian one)
If your 3D printer passes all those criteria, you are good to go!

##### Step 2: Make sure you have the right equipment
Here is a quick rundown:
- 3mm and 3.5mm allen key
- electric screwdriver that can do M3 and M4 SHCs (this is a NECESSITY trust me)
- pliers to remove supports (preferably one that has a pointy tip)
- Flat ground to run it (300m or longer if you want peak performance, no people)

##### Step 3: Source all the stuff (look at the BOM)
Visit the [BOM](https://docs.google.com/spreadsheets/d/1BZxuC8v3igST73ZecLRY6bIY1QTDZrayUpRSoW6Ge5I/edit?usp=sharing) for more info. The BOM should have all the info that you need when sourcing the parts. Make sure that you check that you have all of the stuff bought since there is nothing worse than sitting in front of a almost finished car that cannot run because one bearing is missing. 

##### Step 4: Print everything
Visit the printing guide for more information. Should take ~2d of printing on a X1 Carbon. 

##### Step 5: Assemble and troubleshoot
Follow the manual step by step and you should be fine. The manual should guide you from having a big pile of random stuff in front of you to having a working RC car that drives (hopefully since i am doing more testing). 

### Current problems

1. **Cogging** The motor cogs like nothing else at startup. It functions normally after cogging for a little while but sometimes it cogs a lot and is unable to start. There might be something wrong with the ESC settings (Punch is too high?) and I don't have a program card. The car is already geared up really high so lowering the punch and allowing for a gentler startup may help.
2. **CVs snap** The CVs albeit thicker still have the problem of snapping all the time since it is printed vertically hence the layer lines are screwing it up. I think this is a fundamental limitation of 3D printing and I don't have the ability to come up with a super creative idea to solve it.
3. **Tolerances** 3D printing is a fundamentally not so precise process like CNC machining so tolerances are extremely important. Too tight and eg. the gears bind and the car does not start and too loose everything just refuses to assemble tightly together. I have ironed out a lot of tolerances although it is still a prominent issue. This also highlights the importance of tuning your printer properly. (my printers are actually not so greatly tuned)
4. **Gopro mount** The gopro mount which i tried to design is absolutely horrible and snaps all the time along the layer lines. Even if it doesn't snap it is still horrible since the high g forces make the camera tilt forwards and backwards. Maybe you can help?
5. **Lack of Aero** This is pretty self explanatory as the car currently does not have a proper shell and is just running naked which produces tons of drag. I suck at surface modelling hence everytime I try to design an aerodynamic shell it fails miserebly. This is just a bone that I will have to bite though so stay tuned for any updates.
6. **Unstable** The car is pretty unstable due to the front steering being not perfectly square. This is primarily due to the threaded rods being too short and is a fairly easy fix.
7. **No heat set inserts** The car currently has no heat set inserts which is good for simplicity but terrible when it comes to basically any other aspects. One of the main consequences of this is that parts of the car just either spontaneously comes off or things get wiggly over time. I am currently working on it and stay tuned for updates.

### Background and inspirations

I started this project officially around a year ago because I ran out of stuff to do on a Sunday afternoon. I've had this project idea ever since I started getting into RC cars which is a long time ago and I got inspired to make my own design by Michael Rechtin's high speed RC car project (linked below) and I thought it was an absolute shame that he discontinued it and I decided that I would build a similar project and continue it in my own way. 

### Links

##### Onshape link:
[placeholder]

##### Build guide:
[Link](https://docs.google.com/document/d/1ct8zCZzM1krHP-Pp0RBTua_wGqpxRtsJ6s1tjubo5Lw/edit?usp=sharing)

##### BOM:
[Link](https://docs.google.com/spreadsheets/d/1BZxuC8v3igST73ZecLRY6bIY1QTDZrayUpRSoW6Ge5I/edit?usp=sharing)


##### Tarmo 4:
[Thingiverse](https://www.thingiverse.com/thing:4178426)

##### Tarmo 5:
[Thingiverse](https://www.thingiverse.com/thing:5712880)

### License

This project is a derivative work based on Tarmo 4 and Tarmo 5, 
originally released under CC BY-NC-SA 4.0.

This project is licensed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)**.

You are free to:
- Share — copy and redistribute the material
- Adapt — remix, transform, and build upon the material

Under these terms:
- **Attribution** — You must give credit to the original Tarmo creators AND this derivative author
- **NonCommercial** — You may NOT use this material for commercial purposes
- **ShareAlike** — You must distribute your modifications under the same license

Full license text: https://creativecommons.org/licenses/by-nc-sa/4.0/
