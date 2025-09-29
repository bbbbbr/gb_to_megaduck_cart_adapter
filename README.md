# Game Boy to MegaDuck Cart Slot Adapter
Design files for a plug-in adapter to use Game Boy cartridges on a MegaDuck console.

The consoles have near identical cpu cores (1) and an almost identical cart pinout but a different edge connector style (Game Boy: one-sided, MegaDuck double-sided) and different cartridge widths (MegaDuck cart slot is narrower). This adapter allows plugging GB carts into the MegaDuck Console.

*1. But with modified register addresses, values and other changes to make the MegaDuck incompatible.

![MegaDuck Adapter with a game boy cart connected](/pix/megaduck_gb_to_duck_adapter_cartonly_400.jpg)
![MegaDuck Adapter plugged into a Mega Duck console with a game boy cart connected](/pix/megaduck_gb_to_duck_adapter_console_400.jpg)

# Game Boy game compatibility
- **Q:** Does this mean regular Game Boy carts/games will run unmodified on the Mega Duck with this adapter?
- **A:** __No.__ Game Boy games require manual ROM patching to alter their register addresses, values and other changes in order to run on the Mega Duck.

# Why?
Flash carts for the Game Boy are easier to obtain and are available with a wider variety of features than those for the MegaDuck. Having access to the full range of GB flash carts opens up a lot of options for Mega Duck homebrew development, research and testing. This includes Game Boy Cameras modified to allow running custom ROMs run on them.

# Cartridge Shell
The following 3D printable cartidge shell design can be used with this adapter if the top edge of it is either removed from the design before printing or manually trimmed after printing.

https://github.com/bbbbbr/megaduck_cartridge_shell

TODO: Make cart shell specicially meant for this adapter

# Riser Height
The design has been built with **11mm risers** which provides enough clearance to plug in a some [GB Interceptor](https://github.com/bbbbbr/megaduck-interceptor) builds.

Riser heights down to **3.5mm - 4mm** should work and would result in a much smaller gap between the cart and the back of the console.

# License
Per the LICENSE file this design is released into the public domain and no attribution is required.

# Credits & Thanks
Thanks to Sean Riddle, Nitro2k, TexElec (pcb design)

# Alternate Top Board for Game Boy Camera
A different top board that allows using a regular Game Boy Camera Shell (modified ROM still required) is also available.
It changes the orientation so the Game Boy cart connector is facing UP.

The design is by Raphaël Boichot: https://github.com/Raphael-Boichot/Megaduck-to-game-boy-camera-adapter

# Pix
![MegaDuck Adapter pcb front](/pix/megaduck-front.jpg)
![MegaDuck Adapter pcb rear](/pix/megaduck-rear.jpg)

# GB to MegaDuck Cart Edge Connector Pinout Mapping

| **Mega Duck Cart Side** | **Pin Num** | **GB/DMG Pin** | **Mega Duck Pin** |
| ----------------------- | ----------- | -------------- | ----------------- |
| top                     | 1           | VCC            | +5 VDC            |
| bottom                  | 2           | CLK            | CLK               |
| top                     | 3           | /WR            | /WR               |
| bottom                  | 4           | /RD            | /RD               |
| top                     | 5           | CS             | CS                |
| bottom                  | 6           | A0             | A0                |
| top                     | 7           | A1             | A1                |
| bottom                  | 8           | A2             | A2                |
| top                     | 9           | A3             | A3                |
| bottom                  | 10          | A4             | A4                |
| top                     | 11          | A5             | A5                |
| bottom                  | 12          | A6             | A6                |
| top                     | 13          | A7             | A7                |
| bottom                  | 14          | A8             | A8                |
| top                     | 15          | A9             | A9                |
| bottom                  | 16          | A10            | A10               |
| top                     | 17          | A11            | A11               |
| bottom                  | 18          | A12            | A12               |
| top                     | 19          | A13            | A13               |
| bottom                  | 20          | A14            | A14               |
| top                     | 21          | A15            | A15               |
| bottom                  | 22          | D0             | D0                |
| top                     | 23          | D1             | D1                |
| bottom                  | 24          | D2             | D2                |
| top                     | 25          | D3             | D3                |
| bottom                  | 26          | D4             | D4                |
| top                     | 27          | D5             | D5                |
| bottom                  | 28          | D6             | D6                |
| top                     | 29          | D7             | D7                |
| bottom                  | 30          | /RST           | /RST              |
| top                     | 31          | VIN            | NC                |
| bottom                  | 32          | GND            | NC                |
| top                     | 33          | \-             | NC                |
| bottom                  | 34          | \-             | NC                |
| top                     | 35          | \-             | GND               |
| bottom                  | 36          | \-             | GND               |
