# solve-the-libmpv-error-on-linux
this repo will help you solve libmpv error on linux when trying to run flet main.py
Installing the pakages mpv-libs and mpv-devel on Fedora >=39/41 

Run the command to install the packages:
------------------------------------------------------
``$ sudo dnf install mpv-libs``
------------------------------------------------------
``$ sudo dnf install mpv-devel```
------------------------------------------------------

Searching the packages on directory
------------------------------------------------------
``$ cd /usr/lib64``
------------------------------------------------------

Searching the mpv
------------------------------------------------------
``$ find *mpv*```
------------------------------------------------------

The answer must be:
------------------------------------------------------
``$ libmpv.so libmpv.so.2 libmpv.so.2.1.0```
------------------------------------------------------

Creating a symbolic link
------------------------------------------------------
``$ sudo ln -s /usr/lib64/libmpv.so /usr/lib64/libmpv.so.1``
------------------------------------------------------

ennjoy!
