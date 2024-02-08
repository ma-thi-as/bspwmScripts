# _**BSPMW SCRIPTS**_


**Recomendations: change the group user of /sys/class/backlight/intel_backlight/brightness to your user group**

        sudo chown :mat /sys/class/backlight/{your_card}/brightness
        sudo chmod g+rw /sys/class/backlight/{your_card}/brightness
        
_File ~/.config/sxhkd/sxhkdrc_: \n

XF86MonBrightnessUp

        /home/mat/.config/bspwm/scripts/brightness +1000

XF86MonBrightnessDown \n

        /home/mat/.config/bspwm/scripts/brightness -1000



For battery file is necessary add to crontab
example change first * for the minutes:

* * * * * /home/mat/.config/bspwm/scripts/batt
