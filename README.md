# patchgrade
Nintendo switch patched erista research for 8.01+<br>
Thats also EXTREAMLY DANGROUS.<br>
(this is called a research on getting tegra x1 rcm to load a older signed image, and somehow flashing it)<br>
Yet, if we manage to get it working, it will be very dangrous. You will need to run the exploit AS soon as possible to enable autorcm, and not reboot, cuz if you do, your cooked.<br>
Asuming that the switch wont reboot after updating, it would jump to horizon, witch we have downgraded, somehow... (the bootloader downgrade will be easy, the horizonOS downgrade will be extreamly hard to figure out.
# what the actually f-... i mean, what is this?
Research of downgrading rcm patched eristras and other non rcm exploitable devices to exploitable versions.
# ETA WEN!!!
This is not a utility<br>
I may develop a downgrade utility, if this research comes out successful.
# downgrade guide (UNTESTED), for patched switches, though you will need a rcm exploitable switch. This will probally brick your patched console, and if it dose, follow the unbricking guide below
## IM NOT LIABLE FOR ANYTHING THAT HAPPENS TO YOUR SWITCH! THIS GUIDE IS FOR PEPOLE WHO ARE EXTREAMLY ADVANCED, AND HAVE TIME ON THIER HANDS.
- purchase a switch emmc reader
- take apart your switch
- get to the emmc module, unscrew it, and plug it into the reader
- take a dump of your emmc
- on your other rcm exploitable switch, launch hektate and backup your emmc, and copy it to your computer.
- in hektate enable autorcm on the rcm exploitable switch. (if you dont do this, reflashing the orignal emmc, will be extreamly difficult, since your switch wont even be able to get to rcm, you will need to restore your emmc from the backup and via the emmc reader.
- downgrade the exploitable switches sysnand to 8.0.0
- if you cant get to rcm, you did not enable autorcm, reflash the emmc from the orignal rcm switch backup via the emmc reader, and redowngrade. and enable autoRCM, this is actually extreamly important for the patched switch, you will see why.
- boot into hekate
- dump the emmc and boot0 and bct as rawfiles on the exploitable switch, and copy it to your computer as a seprate filename from the orignal rcm switch backup.
- flash the exploitible switches dump (the one on 8.0.0) via the reader, to your patched switches emmc.
- plug it back into your patched switch, and reasamble it.
- turn on the patched switch, it should show a black screen, and be in rcm mode!
- plug it into your computer, and run nvidias tegrarcm tool (yes they have one) with the bct being the one we dumped from the rcm exploitable switch, and the bootloader as the boot0 we dumped from the rcm exploitable switch
- your patched switch should start booting up, after that follow the switch exploit guide for 8.0.0, and get a payload that enables autorcm, even if the console is patched. boot into the payload to enable autoRCM.
- everytime your patched switch dies, you will need to plug it into your computer, and run nvidias tegrarcm tool (yes they have one) with the bct being the one we dumped from the rcm exploitable switch, and the bootloader as the boot0 we dumped from the rcm exploitable switch
- gointo hektate on the rcm exploitable switch, and flash the orignal emmc.
- Your done!
# unbricking guide
- flash the emmc backup of the switch that bricked itself, to itself, via a external nand reader.
# TODO
- manualy load boot0
