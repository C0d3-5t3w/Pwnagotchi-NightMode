# Pwnagotchi-NightMode

Just changes some colors to make the web ui dark.

# HOW TO

First download this repository. 
Place style.css and the templates folder in the boot partition of your 
sd card with a reader, then pop it in your pi and boot up your pwnagotchi, 
then copy and run the line of commands below and make sure the whole 1 line coppies:

# Commands 

sudo mv /boot/firmware/templates ~ && sudo mv /boot/firmware/style.css ~ && sudo rm ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web/static/css/style.css && sudo rm ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web/templates && sudo mv ~/style.css ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web && sudo mv ~/templates ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web

# What it looks like:

![IMG_0443](https://github.com/user-attachments/assets/bf981448-cd32-40f8-9838-d01080ab75c1)
