# rotarypi
Raspberry Pi Rotary phone // MP3-player

Tested on Raspbian, with a dutch rotary phone


Instructions:

Connect the ground, rotary, rotary-enable and hook switches to the gpios (gnd, 27, 17, 22) of a Raspberry.
Connect the speaker to a usb-soundcard.

Optional: Remove the ringer to get more space inside the phone, add a 18650 battery, 5v boost regulator and tp4056 charger to make it stand-alone)

Install python3, gpiozero, mpg123 and optionally tts (apt-get install ...)

Install this python program, make it executable (chmod +x ./rotarypi/phone.py)

Add mp3s, named [number to dial].mp3

Install cronjob to autostart the script, add an asound setting if you're using an external sound card.
(sudo crontab -e, add the line "@reboot /home/pi/rotarypi/phone.py")




