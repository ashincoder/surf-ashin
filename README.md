# surf-ashin
my suckless browser build.

surf - simple webkit-based browser
==================================
surf is a simple Web browser based on WebKit/GTK+.

Requirements
------------
In order to build surf you need GTK+ and Webkit/GTK+ header files.

In order to use the functionality of the url-bar, also install dmenu[0].

Installation
------------
Edit config.mk to match your local setup (surf is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install surf:

    sudo make clean install

Or install from the aur repository:
      
      yay -S surf-ashin-git ; paru -S surf-ashin-git
      

Running surf
------------
run
	surf [URI]

See the manpage for further options.

Running surf in tabbed
----------------------
For running surf in tabbed[1] there is a script included in the distribution,
which is run like this:

	surf-open.sh [URI]

# Or type this in the terminal:

	tabbed surf -e

Further invocations of the script will run surf with the specified URI in this
instance of tabbed.

[0] http://tools.suckless.org/dmenu
[1] http://tools.suckless.org/tabbed
