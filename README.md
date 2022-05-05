# OpenCVGo
notes on getting started with GoCV

https://github.com/hybridgroup/gocv

## MacOS
On the mac, homebrew may not add the opencv.pc file to the correct location, causing the compile to fail.  If you have this issue, try the following based on your mac processor type.

### M1
On a M1 mac, the following needs to be done after installing both OpenCV and pkg-config.
- cd /opt/homebrew/lib/pkgconfig
- ln -s /opt/homebrew/Cellar/opencv/4.5.5_2/lib/pkgconfig/opencv4.pc opencv4.pc

Note, the version (4.5.5_2) may change based on what is installed.

### Intel
On an Intel mac, the following needs to be done after installing both OpenCV and pkg-config.
- cd /opt/homebrew/lib/pkgconfig
- ln -s /opt/homebrew/Cellar/opencv/4.5.5_2/lib/pkgconfig/opencv4.pc opencv4.pc

Note, the version (4.5.5_2) may change based on what is installed.
- cd /usr/local/lib/pkgconfig
- ln -s /usr/local/Cellar/opencv/4.5.5_2/lib/pkgconfig/opencv4.pc opencv4.pc

