# Qidi-X-Max-3-Configuration
Qidi X-Max 3 Configuration - An attempt to cluster and optimize current config. Make it ready for Klipper 12 native support.



The  Qidi-X-Max-3 is a great machine but regarding software you can find many inconsistencies and non optimal ways of designing the config files.

I assembled a nice set of printer.cfg and macro.cfg that works well and is ready for peer review. I believe there is value for many users and I hope to enhance it further with good quality swarm input.
The following components are included and deviate from standard setup:

Beacon probe instead of other probes --> install
Utilisation of Beacon rev H accelerometer instead of ADXL345 chip
Klippain Shaketune environment to substitue standard input shaper methods
KAMP environment to substitue proprietary Qidi meshing methods
Macros are defined in the macros.cfg
Attention ball screw spindles installed with different rotation distance value! (see stepper_Z section)
All conflicting and non nderstandable code is gone along with dangerous developer functionalities like [force_move]
Use M117 and PRINT_START custom start gcode in slicer
Use PRINT_END custom end gcode in slicer
 
Added components and functions that deviate from Qidi stock setup amongst other:
 [respond], [exclude_object], [gcode_arcs], [idle_timeout],[firmware_retraction],
 PRINT_START and PRINT_END macros with some specifics,
 cleansing of redundant duplettes in config (Fans, Extruder, other...)
Some other stuff is also integrated like tilt_screw_adjust for M4 bolts etc....
