# GCSend
GCSend is a command-line GCode sender for GRBL CNC machines. Compatibility with other GCode-based machines is not guaranteed.

# Installation
GCSend is intended for Linux, but might be easily portable to Windows (i.e. install where you choose, create a shortcut that is on path, or add the installation directory to path.)

```bash
cd /usr/local/bin   # installation directory can be changed
sudo git clone https://github.com/AwesomeCronk/GCSend
sudo chmod 775 GCSend/*
sudo ln -s /usr/local/bin/GCSend/GCSend.py /usr/local/bin/gcsend
```
If your user is not a member of the `dialout` group, you will need to run GCSend as `sudo` to use USB/serial ports. To add yourself to `dialout`, run the following command and then restart your computer:
```bash
sudo usermod -a -G dialout $whoami
```

### Dependencies
* Python 3 (Developed on 3.8.10. Compatibility with other versions not guaranteed.)
* `pySerial` module

# Usage
This section under construction

# Credits
GCSend is based on the [`simple_stream.py`](https://github.com/grbl/grbl/blob/master/doc/script/simple_stream.py) script. The referenced script is Copyright (c) 2012 Sungeon K. Jeon and licensed under the MIT license.