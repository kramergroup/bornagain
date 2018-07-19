# BornAgain

[BornAgain](http://www.bornagainproject.org/) is an Open-source software package to simulate and fit neutron
and x-ray small-angle scattering at grazing incidence.

# Usage

This container is based on [vnc-ubuntu](https://github.com/kramergroup/vnc-ubuntu) and
provides a graphical work environment. It uses [TigerVNC](http://http://tigervnc.org) to
expose an X11 desktop on port 5900 (can be configured).

'''
docker run -it -p 5900:5900 -e USERNAME=born kramergroup/bornagain
'''

This will start a container and use user '''born''' internally to avoid root priviliges
in normal use. The desktop can be accessed with any VNC viewer.

# Installed software

Beside BornAgain, the container has a PyCharm environment ready to use with BornAgain.
