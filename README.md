# My steps


## Day 1

- Pot the plants
- Add some water

## Day 3

- Raspberry Pi Zero W
- Raspberry OS Lite install
  - Use special advanced menu for SSH, Locale, Region, Password
- sudo apt update
- sudo apt upgrade -y
- sudo apt install python3-picamera
- sudo raspi-config
  - Interface Options -> Enable Legacy Camera Support
- sudo raspistill -o image.jpg
- scp pi@raspberrypi.local:~/image.jpg Desktop/
- sudo apt install tmux git -y
- ssh pi@raspberrypi.local
  - git clone https://github.com/alexellis/phototimer
  - mkdir -p ~/image
- cd phototimer
- update config.py
- sudo python take.py 900
