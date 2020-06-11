# What

This snap provides a Qt rutime platform through content interfaces.

# Which Qt

It was built on Ubuntu Bionic and provides the default qt version from the Ubuntu Debian archives. 

Use the snap's `echo` command to inspect the installed enviroment:

    $ sudo snap run --shell test-qt-platform.echo
    $ cd $SNAP

# Shared through snapd content slots

The snap provides Qt to other snaps through several content slots. The other snap needs to have the corresponding content plugs and connect them. 

The consuming application snap also needs various environment variables and snapcraft layouts.

An example that runs a qml: https://github.com/knitzsche/test-qt-app 

# Pi3 tested

This works on Pi3 with Ubuntu Core 18 (armhf).

