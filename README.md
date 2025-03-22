# solve-the-libmpv-error-on-linux #
this repo will help you solve libmpv error on linux when trying to run flet main.py
Installing the pakages mpv-libs and mpv-devel on Fedora >=39/41 

1. Run the command to install the packages:

```$ sudo dnf install mpv-libs```
``$ sudo dnf install mpv-devel```


2. Searching the packages on directory

```$ cd /usr/lib64```


3. Searching the mpv

```$ find *mpv*``` or ```locate libmpv```


The answer must be:

```$ libmpv.so libmpv.so.2 libmpv.so.2.1.0```


4. Creating a symbolic link

```$ sudo ln -s /usr/lib64/libmpv.so /usr/lib64/libmpv.so.1``` 

(change the path based on your case) in my case is /usr/lib64/libmpv.so

ennjoy!
