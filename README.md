# polybar-redshift

## Usage 
Scroll to increase and decrease temperature <br />
Left click to toggle redshift on/off


<img src="https://media.giphy.com/media/cPkE0bq6KMPAUPzikZ/giphy.gif"/>


# Configuration 
Make sure $envFile in redshift.sh points to correct location of env.sh <br />


Add scripts to ~/.config/polybar/scripts and load module from polybar

```
[module/redshift]
type = custom/script
format-prefix = " "  
exec = source ~/.config/polybar/scripts/env.sh && ~/.config/polybar/scripts/redshift.sh temperature 
click-left = source ~/.config/polybar/scripts/env.sh && ~/.config/polybar/scripts/redshift.sh toggle 
scroll-up = source ~/.config/polybar/scripts/env.sh && ~/.config/polybar/scripts/redshift.sh increase
scroll-down = source ~/.config/polybar/scripts/env.sh && ~/.config/polybar/scripts/redshift.sh decrease
interval=0.5
```
