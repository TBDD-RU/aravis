# Install on Ubuntu 16.04, 18.04

* Basic dependencies:

```sh
apt install autoconf intltool gtk-doc-tools libxml2-dev libusb-1.0-0-dev libopencv-dev libcap-ng-dev
```

* GUI (arv-viewer) dependencies:

```sh
apt install libgtk-3-dev libnotify-dev libgstreamer-plugins-base1.0-dev gstreamer1.0-plugins-bad
```

* Build and install:

```sh
./autogen.sh
./configure --prefix=/usr --enable-usb --enable-viewer --enable-gst-0.10-plugin=no
make
make install
```
