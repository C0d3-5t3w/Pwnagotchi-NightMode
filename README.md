# Pwnagotchi-NightMode:

Just changes some colors to make the web ui dark because i dont like so much white.

i butchered the code so please dont try to copy this to the main pwnagotchi repository.

# * The comands below requires you to have an up to date file structure from jayofelony's pwnagotchi fork. *

https://github.com/jayofelony/pwnagotchi.git

# HOW TO:

DISCLAIMER- I am not responsible for the use of and distribution of any pwnagotchi product 
and i do not claim any responsibility for you messing up your files.
everything below worked on multiple fresh installs of jayofelony's fork.

!! First download this repository. !!

Place style.css and the templates folder in the boot partition of your sd card with a reader. 
Then pop it in your pi and boot up your pwnagotchi. 
Copy and run the line of commands below making sure the whole 1 line coppies.

# Commands: 

sudo mv /boot/firmware/templates ~ && sudo mv /boot/firmware/style.css ~ && sudo mkdir -p /boot/firmware/donottrash && sudo mv ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web/static/css/style.css /boot/firmware/donottrash && sudo mv ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web/templates /boot/firmware/donottrash && sudo mv ~/style.css ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web/static/css && sudo mv ~/templates ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web && sync && pwnkill

# What it looks like:

<!--![IMG_0443](https://github.com/user-attachments/assets/f527a735-d376-4ac5-9011-068b7f93b9d1)-->

<!--<img src="https://github.com/user-attachments/assets/f527a735-d376-4ac5-9011-068b7f93b9d1" alt="<3" style="position:relative; width:33%; height:auto;"/>-->

<!--![IMG_0461](https://github.com/user-attachments/assets/ea103e58-24d6-43ef-9748-9d7b3a2c6e18)-->

<img src="https://github.com/user-attachments/assets/ea103e58-24d6-43ef-9748-9d7b3a2c6e18" alt="<3" style="position:relative; width:33%; height:auto;"/>

<!--![IMG_0462](https://github.com/user-attachments/assets/845d1916-edb8-4c74-b5f4-6e7c3fb02ea9)-->

<img src="https://github.com/user-attachments/assets/845d1916-edb8-4c74-b5f4-6e7c3fb02ea9" alt="<3" style="position:relative; width:33%; height:auto;"/>

# Dark Auto-Tune:

In ~/.pwn/lib/python3.11/site-packages/pwnagotchi/plugins/default/auto-tune.py
On line 307 between </title> and <meta add the follow css:

<style>* {color: white; background-color: black;}</style>

# Where:

<!--![IMG_0443](https://github.com/user-attachments/assets/73688345-9e39-4d1f-b1ff-d2940d29a243)-->

<img src="https://github.com/user-attachments/assets/73688345-9e39-4d1f-b1ff-d2940d29a243" alt="<3" style="position:relative; width:50%; height:auto;"/>

# What it looks like:

<!--![IMG_0447](https://github.com/user-attachments/assets/8f18f35c-09e3-44f8-afe1-c3c300c67dee)-->

<img src="https://github.com/user-attachments/assets/8f18f35c-09e3-44f8-afe1-c3c300c67dee" alt="<3" style="position:relative; width:50%; height:auto;"/>

# Black app logo:

Make sure to add pwnagotchi.png to the root of your sdcard just like above

# Run this:

sudo mv /boot/firmware/pwnagotchi.png ~ && sudo mv ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web/static/images/pwnagotchi.png /boot/firmware && sudo mv ~/pwnagotchi.png ~/.pwn/lib/python3.11/site-packages/pwnagotchi/ui/web/static/images && sync && pwnkill

# Colored pwnlog:

Make sure to add conf.colortail to the root of your sdcard just like above

On your pwnagotchi connected to the internet download colortail with:

sudo apt-get install color tail

# Run this:

sudo mv /boot/firmware/conf.colortail ~ && sudo mv /etc/colortail/conf.colortail /boot/firmware && sudo mv ~/conf.colortail /etc/colortail && sync

# Important for pwnlog alias, in /etc/profile change "tail" to "colortail" for pwnlog alias:

<!--![IMG_0463](https://github.com/user-attachments/assets/f133b284-0379-472e-a2e8-ee6db0628f09)-->

<img src="https://github.com/user-attachments/assets/f133b284-0379-472e-a2e8-ee6db0628f09" alt="<3" style="position:relative; width:50%; height:auto;"/>

# What it looks like:
<!--![IMG_0452](https://github.com/user-attachments/assets/fc90304e-ca39-414a-a3ad-05779de90c17)-->

<img src="https://github.com/user-attachments/assets/fc90304e-ca39-414a-a3ad-05779de90c17" alt="<3" style="position:relative; width:50%; height:auto;"/>

<!--![IMG_0453](https://github.com/user-attachments/assets/61bebba6-21bc-4cec-b72b-efe74ce7e935)-->

<img src="https://github.com/user-attachments/assets/61bebba6-21bc-4cec-b72b-efe74ce7e935" alt="<3" style="position:relative; width:50%; height:auto;"/>

# We could also pipe pwnlog through color tail:

On your pwnagotchi connected to the internet download lolcat with:

sudo apt-get install color tail

# Add "| lolcat" to the end of pwnlogs alias in /etc/profile here:

# What it looks like: 🤢

# ENJOY!!! if you have any issues find and @ me in the pwnagotchi unofficial discord: https://discord.gg/wBgZPn6M