Intel® XDK IoT Node.js\* I2C Peripheral Interface App
=====================================================

See [LICENSE.md](LICENSE.md) for license terms and conditions.

This sample application is distributed as part of the
[Intel® XDK](http://xdk.intel.com). It can also be downloaded
or cloned directly from its git repo on the
[public Intel XDK GitHub\* site](https://github.com/gomobile).

For help getting started developing applications with the
Intel XDK, please start with
[the Intel XDK documentation](https://software.intel.com/en-us/xdk/docs).

See also, the
[mraa library documentation](https://iotdk.intel.com/docs/master/mraa/index.html)
for details regarding supported boards and the mraa library API and the
[upm library documentation](https://iotdk.intel.com/docs/master/upm/) for
information regarding the upm sensor and actuator library APIs.

App Overview
------------

This example drives a JHD1313m1 LCD as found in the Grive Starter Kit. This
connects to an i2c buss. It demonstrates the use if the i2c bus. Note that the
code will depend on the device you are driving as much as it depends upon the
bus.

Still, there is some useful code that you can use in this example.  The
purpose of this template is to demonstrate driving the i2c buss directly from
Javascript. Notice that we need delays between some of the bus transactions.
If you were writing in C, you could use the wait system call, but there is no
direct equivalent to "wait" in Javascript. Instead we have to set up a
callback on a timer. So i2c.js creates a queue driven execution engine for i2c
devices.

Important App Files
-------------------

* main.js
* i2c.js
* package.json

Important Project Files
-----------------------

* README.md
* LICENSE.md
* \<project-name\>.xdk

Tested IoT Node.js Platforms
----------------------------

* [Intel® Galileo Board for Arduino](http://intel.com/galileo)
* [Intel® Edison Board for Arduino](http://intel.com/edison)

This sample can run on other IoT [Node.js](http://nodejs.org) development
platforms, that include the appropriate sensor hardware, but may require
changes to the I/O initialization and configuration code in order to work on
those other platforms.
