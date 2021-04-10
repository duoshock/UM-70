# UM-70 Assembly Guide

## **Content of UM-70 Kit**

<a href="images/00_WhatsInTheBox.jpg">
<img src="images/00_WhatsInTheBox.jpg" width="400">
</a>

**Housing** 
- 2 x Top Case
- 2 x Rear Cover
- 2 x Side Panel
- 1 x Rotary Encoder Knob

**RF4 Plate**
- 1 x Left
- 1 x Right

**1 x OLED Screen PCB**

**1 x OLED Screen**

**2 x 4 Pins Sockets**

**1 x 4 Pins Cable**

**1 x Encoder**

**100 x SK6812MINI RGB LED** (Only 86/87 are required, rest are spare)

**80 x Hot swap sockets** (Only 70/71 are required, rest are spare)

**2 x TRRS PJ-320A**

**20 x M2 3mm screws** (Only 16 are required, rest are spare)

**10 x M2 3mm Standoffs** (Only 8 are required, rest are spare)

**10 x M2 washers** (Only 8 are required, rest are spare)

**15 x M3 5mm screws** (Only 13 are required, rest are spare)

**10 x M3 14mm screws** (Only 8 are required, rest are spare)

**4 x M3 DIN562 Square Nuts** (It’s used as thread insert under the mounting points, all square nuts are already inserted to the case before shipping, but it may come loss during shipping or may have missed. In that case here are the spare)

**10 x Rubber feet** (Only 8 are required, rest are spare)

## **Test the main PCBs before soldering**

<a href="images/01_Test.jpg">
<img src="images/01_Test.jpg" width="400">
</a>

All PCBs are tested prior shipping, but it’s a good practice to make sure it’s working before soldering. It should be recognised as keyboard when plugged, test it by shorting switch pins with tweezers. Don’t panic if the right side PCB outputted wrong keys, as the firmware is set to left as master. I.e. USB cable should be connected to left half when in use.



## **Assembling the Main PCBs**

<a href="images/02_LEDs.jpg">
<img src="images/02_LEDs.jpg" width="400">
</a>

**_Blue = In-switch LEDs_**

**_Orange = Panel LEDs_**

There’re 33 in-switch and 6 for panel LEDs on the left half. 37 in-switch (38 for split backspace) and 6 panel LEDs on the right side.


## **Panel LEDs**

<a href="images/03_PanelLEDLens.jpg">
<img src="images/03_PanelLEDLens.jpg" width="400">
</a>

<a href="images/04_PenalLEDMarking.jpg">
<img src="images/04_PenalLEDMarking.jpg" width="400">
</a>

To solder side panel LED, LED lens should be faced up. Align the marking on the PCB and the LED, repeat the same process to the rest.

## **In-switch LEDs**

<a href="images/06_SwitchLEDMarking_A.jpg">
<img src="images/06_SwitchLEDMarking_A.jpg" width="400">
</a>

<a href="images/06_SwitchLED_B.jpg">
<img src="images/06_SwitchLED_B.jpg" width="400">
</a>

To solder in-switch LED, LED lens should be facing down, align the markings on the PCB and the LED.


<a href="images/07_Layout_Left.jpg">
<img src="images/07_Layout_Left.jpg" width="400">
</a>

<a href="images/07_Layout_Right.jpg">
<img src="images/07_Layout_Right.jpg" width="400">
</a>

When solder LEDs for spacekey on the left, and Backspace on the right, only solder the to one layout.

## **Hot swap sockets**
<a href="images/08_Hotswap_A.jpg">
<img src="images/08_Hotswap_A.jpg" width="400">
</a>

Place sockets like it shown in the photo. When soldering sockets for Spacekey and Backspace, only solder sockets to one layout only, refer previous step for placements.


<a href="images/09_RightHowswap_A.jpg">
<img src="images/09_RightHowswap_A.jpg" width="400">
</a>

There’re 4 sockets on the edge of the right half need modifications on the hot swap sockets.

<a href="images/09_RightHowswap_B.jpg">
<img src="images/09_RightHowswap_B.jpg" width="400">
</a>
<a href="images/09_RightHowswap_C.jpg">
<img src="images/09_RightHowswap_C.jpg" width="400">
</a>

Speare the right pin of the socket like it shown the photo and then solder.


## **TRSS Jacks**
<a href="images/10_TRRS_A.jpg">
<img src="images/10_TRRS_A.jpg" width="400">
</a>
<a href="images/10_TRRS_B.jpg">
<img src="images/10_TRRS_B.jpg" width="400">
</a>

Place the jack on the back of the PCB, then solder at the front.

## **OLED Screen Connector**
<a href="images/11_OLEDSocket_A.jpg">
<img src="images/11_OLEDSocket_A.jpg" width="400">
</a>

The connector is located on the left half

<a href="images/11_OLEDSocket_B.jpg">
<img src="images/11_OLEDSocket_B.jpg" width="400">
</a>
<a href="images/11_OLEDSocket_C.jpg">
<img src="images/11_OLEDSocket_C.jpg" width="400">
</a>

Insert it on the back of the PCB, then solder at the front.

---

## **Buzzer**
_Optional, AST1109MLTRQ buzzer is not included in the kit_

<a href="images/12_Buzzer_A_L.jpg">
<img src="images/12_Buzzer_A_L.jpg" width="400">
</a>
<a href="images/12_Buzzer_A_R.jpg">
<img src="images/12_Buzzer_A_R.jpg" width="400">
</a>

Buzzers are located at the front of the PCBs, only solder buzzer on the master half (Left half by default).

_QMK does not support speaker on the on salve half. Audio is not enabled by default. Buzzer is wired to IO pin B6._

<a href="images/12_Buzzer_B.jpg">
<img src="images/12_Buzzer_B.jpg" width="400">
</a>
<a href="images/12_Buzzer_C.jpg">
<img src="images/12_Buzzer_C.jpg" width="400">
</a>

AST1109MLRQ is non-polarity, solder anyway up.


## **Test the PCBs**

Connect both halves with TRRS cable first, and then connect USB cable to the left half.

**DO NOT PLUG/UNPLUG TRRS CABLE WHEN POWER IS ON (I.E. WHEN USB CABLE IS CONNECTED), IT WILL SHORT THE CONTROLLER AND MAY KILLS IT.**

Check all LEDs are working before proceeding to next step.
