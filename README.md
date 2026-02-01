# PDP1-Dpy-SDL2
A Type 30 display for the PiDP1
This is a Linux app tested under Raspbian Bookworm running on a Raspbery Pi 3B.
It is based upon Simh and contains only the relevant files to build a pdp1 simh app.
It is intended as an optional Type 30 display for the PiDP1 (real hardware or virtual).
I have set this app up to display on a cheap and cheerful 1280x1024 display:
The graphics system (SDL2) is the same as that used for the PiDP11 and the GT40 display system that may be used with the PiDP10.

1. Clone this repo:
git clone https://github.com/Isysxp/PDP1-Dpy-SDL2.git
2. Install SDL2 on your pi:
sudo apt install libsdl2dev
3. In the PDP1-Dpy_SDL2 directory:
make pdp1
4. Run the app, in the BIN directory type:
./pdp1
4. Start the PiDP1 machine in 'apps' mode (see the instructions in the handbook).
5. Close the P7 sim window as we will be using the pdp1-dpy app for the display
6. Start you favourite app on the PiDP1 machine eg dpys5-demo.rim
7. At the sim prompt on the display machine:
sim> set dpy ena
sim> att dpy pidp1 (where pidp1 is the name of your PiDP1 machine)<br>
And you should see:
![Project Screenshot](Assets/screenshot.jpeg)


