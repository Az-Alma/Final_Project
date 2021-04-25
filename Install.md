# Final_Project
This is the software I used for my senior project in cyber security II
This setup was done on a MacOs device.

### Requirements Before Installing Rfcat.

# download via curl
$ curl -L -C - "https://github.com/libusb/libusb/releases/download/v1.0.24/libusb-1.0.24.tar.bz2" -o ~/Downloads/libusb-1.0.24.tar.bz2

# unzip archive
$ tar -xf ~/Downloads/libusb-1.0.24.tar.bz2 -C ~/Downloads/

# change into extraced archive directory
$ cd Downloads/libusb-1.0.24

# verify dependencies for build and install process are available
$ ./configure

# run build
$ make

# run installation
$ sudo make install

# verify installation (optional)
$ ls -la /usr/local/lib/libusb*

# delete archive and directory (optional)
$ rm -fr ~/Downloads/libusb-1.0.24*


##Pyhton Install

# install libusb via pip
$ python2.7 -m pip install libusb

# install pyusb via pip
$ python2.7 -m pip install pyusb

# install pyreadline via pip
$ python2.7 -m pip install pyreadline

# install ipython via pip
$ python2.7 -m pip install ipython

# install PySide2 via pip
$ python2.7 -m pip install PySide2


##RFcat Install

# clone from GitHub
$ git clone https://github.com/atlas0fd00m/rfcat.git ~/Downloads/rfcat

# change directory
$ cd Downloads/rfcat

# run the installation
$ sudo python2.7 setup.py install

# verify the installation (optional)
$ ls -la /usr/local/bin/rfcat*

# show rfcat help (optional)
$ /usr/local/bin/rfcat -h

# delete cloned directory (optional)
$ rm -fr ~/Downloads/rfcat


###ooktools

# install ooktools via pip
$ python2.7 -m pip install ooktools

# verify and show help (optional)
$ python2.7 -m ooktools.console --help

# verify and show specific help topic (optional)
$ python2.7 -m ooktools.console wave --help


###Run Rfcat

$ sudo rfcat -r
