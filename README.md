ABOUT:
- This is my modified version of qpaeq
- For a midi controller I am using korg nanoKONTROL2
- My goal is to code qpaeq to recognize midi input in order to control 
the equalizer.

WHAT WORKS:
- compiles with midi support
- no functionality yet

REQUIRES:
- qt4-*
- libjack-dev
- python-rtmidi

SOME UBUNTU COMMANDS:
	sudo add-apt-repository ppa:webupd8team/pulseaudio-eq
	sudo apt-get update

	sudo apt-get install python-dbus python-qt4 python-qt4-dbus pulseaudio-utils

	pulseaudio -k
	pulseaudio --start

	pactl load-module module-equalizer-sink
	pactl load-module module-dbus-protocol

USAGE:
	./qpaeq.py
