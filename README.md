# v0-870-klipper_config

![V0.1-870](./images/v0.1-870.jpg)

Klipper configs for this printer running fluidd.

# Table of Contents
**(!)** = has important warning
- [**(!)** Change Log](#change-log)
- [Printer Mods](#printer-mods)
- [Klipper Plugins](#klipper-plugins)

# Change Log

Changes will be noted here by date, title if needed, files changed, summary of changes. 

_**Note: only changes of signifigance will be added.**_


- **24-11-2021:** Initial placeholder of changelog layout
    * Enabled
        * `configs/dockable_probe.cfg`
        * `configs/z_calibration.cfg`
    * Disabled
        * `configs/probe.cfg`
	* `configs/bed_mesh.cfg` 
        * Use dense bed mesh
            * `probe_count: 5,5` -> `probe_count: 9,9`
            * `relative_reference_index: 24` -> `relative_reference_index: 77`

# Printer Mods

* [Timmit's klipper expander](https://github.com/VoronDesign/Voron-Hardware/tree/master/Klipper_Expander)
* [Timmit's umbilical pcb's](https://github.com/VoronDesign/Voron-Hardware/tree/master/V0-Umbilical)
* [Timmit's v0 display](https://github.com/VoronDesign/Voron-Hardware/tree/master/V0_Display)
* [221 wago mount for bed](https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/BlueBear/Wago_221_mount)
* [NeverMore v5 duo](https://github.com/nevermore3d/Nevermore_Micro/tree/master/V5_Duo/V0)
* [1515 snap in led mounts](https://github.com/newphreak/VoronUsers/tree/1515ledmod/printer_mods/Jon/1515_led_mount)



# Klipper Plugins

* gcode_shell_command

# Credits in no particular order

* [eecue's klipper_configs](https://github.com/eecue/klippper-config)
* [zellneralex's klipper_configs](https://github.com/zellneralex/klipper_config)
* [FHeilmann's klipper_configs](https://github.com/FHeilmann/klipper_config/)
* [th33xitus/kiauh klipper github backup](https://github.com/th33xitus/kiauh/wiki/How-to-autocommit-config-changes-to-github%3F)
