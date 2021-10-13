# v0-870-klipper_config

Baby blue's config.

Credits to [eecue](https://github.com/eecue/klippper-config) where most comes from, and [Jasrags](https://github.com/Jasrags/V2-1031-klipper_config) for another big chunk. Just don't let them look at it, they will certainly cry.






# KLIPPER CONFIG BACKUP SCRIPT HOWTO
- `ssh-keygen`
- `cat ~/.ssh/id_rsa.pub`
- add to "ssh and gpg keys" on github
- make `.gitignore` file in klipperconfig and put in `printer-*_*.cfg`
- Get KIAUH and install shell command extension
  ```
  wget https://raw.githubusercontent.com/newphreak/V2-1755-klipper_config/main/autocommit.sh
  cd ~
  git clone https://github.com/th33xitus/kiauh.git
  ./kiauh/kiauh.sh
  ```
  Go to (4) Advanced and install the shell command extension (9) (Select yes for everything)
- Put this in printer.cfg or wherever you have macros:

  ```
  [gcode_shell_command backup_cfg]
  command: sh /home/pi/klipper_config/autocommit.sh
  timeout: 30.0
  verbose: True
  [gcode_macro BACKUP_CFG]
  gcode:
  RUN_SHELL_COMMAND CMD=backup_cfg
  ```

- Go back to github and create a new repository (+ menu on the top right corner) and select new repository)

  Use the `<printer type>-<serial>-klipper_config` naming scheme
- Follow the instructions for pushing readme.md **BUT DO MAKE SURE YOU'VE SELECTED SSH AND NOT HTTP**, do this from ~/klipper_config
- Go to to fluidd/mainsail and run the backup_cfg macro.

  Voilà.
