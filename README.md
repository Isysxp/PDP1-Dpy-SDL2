# PDP1-Dpy-SDL2
A Type 30 display for the PiDP1
This is a Linux app tested under Raspbian Bookworm running on a Raspbery Pi 3B.
It is based upon Simh and contains only the relevant files to build a pdp1 simh app.
It is intended as an optional Type 30 display for the PiDP1 (real hardware or virtual).
I have set this app up to display on a cheap and cheerful 1280x1024 display:
The graphics system (SDL2) is the same as that used for the PiDP11 and the GT40 display system that may be used with the PiDP10.

1. clone this repo:
git clone 
3. install SDL2 on your pi:
sudo apt install libsdl2dev
Then in the PDP1-Dpy_SDL2
