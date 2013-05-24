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


Using debuild to generate signed packages
=========================================

The folder has to be renamed to package name.

    whonix-gateway-1.0.0

Instead of running fakeroot run debuild with your generated user id.

    debuild -k 'Bao Nguyen <nguybao@yahoo.com>'

If you are new to gpg you can generate you key as follow, but you need to run it only once:

    gpg --gen-key