                               xroot

xroot runs a command every time a given mouse button is pressed on
the root window.

§ Installation

In order to build xroot you need the Xlib header files.

Edit config.mk to match your local setup (xroot is installed into
the /usr/local prefix by default).  Then enter the following command to
build and install xroot (if necessary as root).

	make clean install

§ Running xroot

xroot gets as argument an command and its arguments and run this
command every time the right mouse button is pressed on the root window.

One of the options -l, -m, -r, -1, -2, -3, -4, or -5 can be  passed as
first argument.  Those options indicates, respectivelly, that the left,
middle, right or N-th mouse button is to be used instead.

Call xroot on your .xinit or .xsession file in background, before
the window manager.  As the following:

	xroot -l xterm &

Read the [manual](https://github.com/the-repo-club/xroot/wiki) for more information on running xroot
