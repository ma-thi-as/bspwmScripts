# _**BSPMW SCRIPTS**_


For brightness file is necessary add to sudoers the command "tee" 

_File ~/.config/sxhkd/sxhkdrc_: \n
XF86MonBrightnessUp
        /home/mat/.config/bspwm/scripts/brightness +1000

XF86MonBrightnessDown \n
        /home/mat/.config/bspwm/scripts/brightness -1000



For battery file is necessary add to crontab
example change first * for the minutes:
* * * * * /home/mat/.config/bspwm/scripts/batt
