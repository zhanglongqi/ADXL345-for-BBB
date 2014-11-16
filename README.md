Beagleboneblack I2C ADXL345 Accelerometer
========================================+

This is a demonstartion implemenation of Beaglebone Black and ADXL345 accelerometer using the i2c bus. The program and 
demonstrates the how set up the ADXL345 accelerometer as well as access X, Y and Z data. The roll and pitch outputs
accessed.

##enable the hardware interrupt
The ADXL345 have two interrupts pin, in this case, only one is used, `INT-1` is used as the interrupt source to inform 
the system. it connect with `GPIO2_1(HardWware)`, actually it's GPIO3 in the device tree or in the linux kernel, it should
be the mistake of dvice tree writer, they are GPIO 1,2,3,4 instead of the GPIO 0,1,2,3. this really confuse me for hours.

