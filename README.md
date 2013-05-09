Whonix-build
============

Build source code for project Whonix.

To make build:

    git clone Whonix

    git clone Whonix-build

copy over these folders: whonix_gateway, whonix_shared, whonix_workstation
so that they are corresponding to Whonix-build folders: whonix_gateway, whonix_shared, 
whonix_workstation
then from each folder run:

    fakeroot debian/rules binary

