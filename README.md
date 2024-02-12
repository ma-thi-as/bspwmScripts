# _**BSPMW SCRIPTS**_


**Recomendations: change the group user and perms of /sys/class/backlight/{your_card}/brightness to your user group**
        
        if u have intel_backlight in the command """ls /sys/class/backlight"""
        sudo chown :mat /sys/class/backlight/intel_backlight/brightness
        sudo chmod g+rw /sys/class/backlight/intel_backlight/brightness
        
_File ~/.config/sxhkd/sxhkdrc_:

        XF86MonBrightnessUp

                        /home/mat/.config/bspwm/scripts/brightness +1000


        XF86MonBrightnessDown

                        /home/mat/.config/bspwm/scripts/brightness -1000


_For battery file is necessary add to crontab -e
example change first * for the minutes_

        * * * * * /home/mat/.config/bspwm/scripts/batt
        
