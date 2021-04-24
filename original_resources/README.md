# Original resources

Laser Cube was a [Kickstarter project](https://www.kickstarter.com/projects/820277733/laser-cube) in 2014. It's still accessible but just in case here is [a pdf snapshot](laser_cube_kickstarter_snapshot.pdf).

From kickstarter we learn that their main site was www.littlegeektoys.com (now down) and it was operating GRBL with Grbl Controller 3.61 to Send G-code to the machine.

[littlegeektoys on archive.org](https://web.archive.org/web/20161025014426/http://www.littlegeektoys.com/) and [pdf snapshot](littlegeektoys.pdf).

Some videos, G-Code examples and resources found on the Kickstarter actus & comments.

## Videos

* [Laser Cube Assembly](http://youtu.be/YLJizU0NRb4)
* [Laser Cube X Axis Assembly](http://youtu.be/rCOG-0a0hg8)
* [Laser Cube Y Axis Assembly](http://youtu.be/jpPKOWAiQHA)
* [LaserCube Instructions](https://www.youtube.com/watch?v=3PbqsSkWJyk)
* [LaserCube engraving Cell phone Case](https://www.youtube.com/watch?v=0kG5Q0Zs49Q)
* [LaserCube cut foam board](https://www.youtube.com/watch?v=ZiN_rVVj4DM)
* [LaserCube](https://www.youtube.com/watch?v=9zkb4mIJ67s)
* [LaserCube](https://www.youtube.com/watch?v=7eu3_24YkjE)
* [LaserCube](https://www.youtube.com/watch?v=tFGP2bx-m5w)

## Examples

* [My Neighbor Totoro.nc](https://www.dropbox.com/s/m8epaybr3raq9vu/My%20Neighbor%20Totoro.nc?dl=0), [local copy](examples/My_Neighbor_Totoro.nc)
* [Eagle.nc](https://www.dropbox.com/s/6ehigvxhnima3oy/Eagle.nc?dl=0), [local copy](examples/Eagle.nc)
* [MJ.nc](https://www.dropbox.com/s/h7crqrkh0y7xjrr/MJ.nc?dl=0), [local copy](examples/MJ.nc)
* [PacMan A.nc](https://www.dropbox.com/s/9oghnsu0albwzen/PacMan%20A.nc?dl=0), [local copy](examples/PacMan_A.nc)
* [PacMan B.nc](https://www.dropbox.com/s/ase9e9k221ejaeu/PacMan%20B.nc?dl=0), [local copy](examples/PacMan_B.nc)
* [PacMan C.nc](https://www.dropbox.com/s/ofit8asil9wxbxp/PacMan%20C.nc?dl=0), [local copy](examples/PacMan_C.nc)
* [PacMan D.nc](https://www.dropbox.com/s/2h1xq5uof9q03xl/PacMan%20D.nc?dl=0), [local copy](examples/PacMan_D.nc)

## Procedures

### Tuning Steppers

X and Y axis steppers have a potentiometer to make the stepping motor running smoothly
* CW to increase the current strength. If too strong, it could make the cube a little hot
* CCW to decrease the current strength. If too weak, the motor could make some "noise" (skip steps?)

### Homing, for the .nc examples above:

* Focus your laser on the target material
* Gently use your hand push the X axis to the end of right hand side. 
* The Y is pulled all the way towards to you (in front). 
* After that, you click (Zero Position) button in the Grbl controller.

### GCode

Based on Grbl 0.6b? Some kickstarter comments mentioned Grbl 0.8c as well. 9600 bauds.

* M3 turns laser on, M5 turns laser off

*Please remember, don't unplugged the USB while the laser working . it could destroy sth.*


* [Grbl at dank.bengler.no](http://dank.bengler.no/-/page/show/5470_grbl) (dead), [archive.org](https://web.archive.org/web/20190616194514/http://dank.bengler.no:80/-/page/show/5470_grbl) => mentions repo at http://github.com/grbl/grbl

* [Simen repo](https://github.com/simen/grbl) => mentions repo at http://github.com/grbl/grbl

* [grbl/grbl repo](http://github.com/grbl/grbl) => mentions repo at https://github.com/gnea/grbl

## Zapmaker Grbl Controller

*It has been written as a superior replacement for the popular GCodeSender, and UniversalGCodeSender.*

But the author disappeared around July 2014.

* [Grbl Controller 3.61 wiki](http://www.shapeoko.com/wiki/index.php/Grbl_Controller) => [new link](https://wiki.shapeoko.com/index.php/Grbl_Controller)
* [Grbl Controller Downloads](http://zapmaker.grblcontroller.s3-website-us-west-2.amazonaws.com/)(dead), [archive.org](https://web.archive.org/web/20140628054314/http://zapmaker.grblcontroller.s3-website-us-west-2.amazonaws.com/)
* [sources](https://github.com/zapmaker/GrblHoming/), [Github wiki](https://github.com/zapmaker/GrblHoming/wiki)

### Windows
* [GrblController361Setup.exe](http://zapmaker.grblcontroller.s3-website-us-west-2.amazonaws.com/GrblController361Setup.exe) (dead), [archive.org](https://web.archive.org/web/20140718182637/http://zapmaker.grblcontroller.s3-website-us-west-2.amazonaws.com/GrblController361Setup.exe)
* Windows CH341 driver [CH341SER.ZIP](http://www.wch.cn/downfile/5) (dead), [archive.org](https://web.archive.org/web/20180410140345/http://www.wch.cn:80/downfile/5), [local copy](GrblController/CH341SER.ZIP)

### Mac
* [GrblController35.dmg](http://zapmaker.grblcontroller.s3-website-us-west-2.amazonaws.com/GrblController35.dmg) (dead), [archive.org](https://web.archive.org/web/20140628054314/http://zapmaker.grblcontroller.s3-website-us-west-2.amazonaws.com/GrblController35.dmg)
* Mac CH341 driver [CH341SER_MAC.ZIP](http://www.wch.cn/downfile/5) (dead), [archive.org](https://web.archive.org/web/20180410140345/http://www.wch.cn:80/downfile/5), [local copy](GrblController/CH341SER_MAC.ZIP)

### Linux

* [GrblControllerLinuxInstallerx86-3.6.1](http://zapmaker.grblcontroller.s3-website-us-west-2.amazonaws.com/GrblControllerLinuxInstallerx86-3.6.1) (dead), [archive.org](https://web.archive.org/web/20140628054314/http://zapmaker.grblcontroller.s3-website-us-west-2.amazonaws.com/GrblControllerLinuxInstallerx86-3.6.1)
* [GrblControllerLinuxInstallerx64-3.6.1](http://zapmaker.grblcontroller.s3-website-us-west-2.amazonaws.com/GrblControllerLinuxInstallerx64-3.6.1) (dead), [archive.org](https://web.archive.org/web/20140628054314/http://zapmaker.grblcontroller.s3-website-us-west-2.amazonaws.com/GrblControllerLinuxInstallerx64-3.6.1)

* `sudo apt-get install "^libxcb.*" libx11-xcb-dev libglu1-mesa-dev libxrender-dev`
* chmod 755 the installer file you downloaded so you can run it
* After installing, GrblController executable will be found in ~/GrblController folder:

### Tips

To remove the "Alarm lock", please go to the " Advance" of Grbl controller , under the "Reset control ", and click the "unlock Grbl"

## Pocket Laser Engraver

It's a similar project and Laser Cube mentions its **Step 7** for creating and sending GCode. The same steps were mentioned on the defunct www.littlegeektoys.com

* [Pocket Laser Engraver on instructables](https://www.instructables.com/Pocket-laser-engraver/)
* Laser engraver extension of Inkscape: [laserengraver.zip](http://www.slackersdelight.com/instructables/laserengraver.zip) ([local copy](inkscape/laserengraver.zip)), heavily modified version of [Gcodetools](http://www.cnc-club.ru/forum/viewtopic.php?f=15&amp;p=101)
* G-code sender [gcodesender.exe](https://github.com/downloads/OttoHermansson/GcodeSender/gcodesender.exe), sources [on GitHub](https://github.com/OttoHermansson/GcodeSender)
* [files](https://www.slackersdelight.com/instructables/)

About compiling the firmware:

*After downloading and extracting the code you have to change the port numbers in config.h and make sure you get them in the right order. Then all you have to do is start a command window, enter the correct folder and type "make". If all goes to plan you should end up with a .hex file ready for the Arduino.
I have however changed the pin-out since then and here in the instructable I use the default pin-out of Grbl.*

*The current version of Grbl (0.6b) has a bug in the queue system. The laser on and off (M3, M5) commands are not put in the queue and the laser will be turned on and off as soon as the Arduino receives the commands. This is resolved in the edge branch.  https://github.com/simen/grbl/tree/edge*

But that branch doesn't exist anymore, neither in the forks.

```
Grbl 0.6b
'$' to dump current settings"
```
If you enter $ followed by return you will get a list of options. Something like this:
```
$0 = 400.0 (steps/mm x)
$1 = 400.0 (steps/mm y)
$2 = 400.0 (steps/mm z)
$3 = 30 (microseconds step pulse)
$4 = 480.0 (mm/sec default feed rate)
$5 = 480.0 (mm/sec default seek rate)
$6 = 0.100 (mm/arc segment)
$7 = 0 (step port invert mask. binary = 0)
$8 = 25 (acceleration in mm/sec^2)
$9 = 300 (max instant cornering speed change in delta mm/min)
'$x=value' to set parameter or just '$' to dump current settings
ok
```
*You must change the steps/mm for X and Y axis to 53.333 on both. Just enter "`$0=53.33`" followed by return and then "`$1=53.333`" followed by return. Z axis can be ignored as it is not used. The acceleration can be ramped up to something like 100 ("`$8=100`" and return). As we move really slowly with this machine acceleration can be high. Another side effect of low acceleration can be that curves get a lot more burnt than straight lines as the controller constantly tries to accelerate and decelerate but never reach full speed. If you build this like me one of your axis might be mirrored. This is easy to fix. Option `$7` lets you change direction on axis. I wanted to change direction on the X axis so I type in "`$7=8`" as I want to change bit 3 (8 = 00001000 binary) if you want to change direction on Y axis you type in 16 (00010000) or 24 (00011000) to change both.*

*The complete documentation of the invert mask can be found here http://dank.bengler.no/-/page/show/5474_configuringgrbl* (dead), [archive.org](https://web.archive.org/web/20190616191050/http://dank.bengler.no:80/-/page/show/5474_configuringgrbl)

*Now you are ready for the computer setup. If you want to try some movement you can type "`G91 G28 X0 Y0 [return]`" to zero the axis. Followed by "`X10 Y10 [enter]`". You should see 10mm movement on each of the axis.*

