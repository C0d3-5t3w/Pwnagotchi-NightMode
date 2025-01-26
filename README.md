# Pwnagotchi-NightMode:

Just changes some colors to make the web ui dark because i dont like so much white.

# * The comand below requires you to have an up to date file structure from jayofelony's pwnagotchi fork. *

# HOW TO:

First download this repository.

Place style.css and the templates folder in the boot partition of your sd card with a reader. 
Then pop it in your pi and boot up your pwnagotchi. 
Copy and run the line of commands below making sure the whole 1 line coppies.

# Commands: 

sudo mv /boot/firmware/templates ~ && sudo mv /boot/firmware/style.css ~ && sudo mkdir -p /boot/firmware/donottrash && sudo mv ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web/static/css/style.css /boot/firmware/donottrash && sudo mv ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web/templates /boot/firmware/donottrash && sudo mv ~/style.css ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web/static/css && sudo mv ~/templates ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web && sync && pwnkill

# What it looks like:

![IMG_0443](https://github.com/user-attachments/assets/f527a735-d376-4ac5-9011-068b7f93b9d1)
