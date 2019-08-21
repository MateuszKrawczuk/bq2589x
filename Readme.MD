# BQ2989x driver for TI BQ2589X battery charger

* Supported kernel: 4.18 and newer

bq2589x driver supports bq25890/bq25892/bq25895 series chip.
but some configuration and parameters are different, so we
need note specific difference between the chips.


## Compile
To make and make install module for BQ2589X driver:

> KDIR=\<your kernel source path> make

> KDIR=\<your kernel source path> INSTALL_MOD_PATH=\<absolute path of kernel module> make modules_install

(NOTE: The "modules" directory should be already installed kernel module inside)

## Load module driver

Load the module driver on the board:

> modprobe bq2989x-charger
