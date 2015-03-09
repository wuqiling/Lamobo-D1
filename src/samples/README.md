#Lamobo D1s Samples Codes

## Building Samples

Before building, please make sure that **arm-none-linux-gnueabi-gcc** is in PATH.

To build, type '**make**'.

To clean, type '**make clean**'.

## Invoking Samples

Just copy them to the TF card.

## Using Samples

-  **gpio-led**: The gpio sample makes led blinking 3 times.

-  **i2c-test**: To access i2c device, you can just use opensource i2c tools, or this demo. For example how to read and write rtc(ds1307) device:
    - rtc registed on 0x68, and we read from 0x0 to 0x12.
        - ./i2c-test r 0x68 0 0x12
    - set minute to 49.
        - ./i2c-test w 0x68 0x1 0x49