Old Grbl versions: `screen /dev/ttyUSB0 9600`  

### Grbl v0.6 test

From https://github.com/grbl/grbl

```
git checkout -b v0_6 origin/v0_6
make
-> compilation error
```

### Grbl v0.7 test

From https://github.com/grbl/grbl

```
git checkout -b v0_7 origin/v0_7
make
avrdude -c arduino -P /dev/ttyUSB0 -b 57600 -p atmega328p -B 10 -U flash:w:grbl.hex:i
screen /dev/ttyUSB0 9600
$
$0 = 72
$1 = 72
$8 = 100

G0 X10 Y10
G0 X0 Y0
```
It moves !!
`$7` to inverse axes seems to not have effect

72 steps/mm was found experimentally, maybe not the exact value.

### Grbl v0.8c test

From https://github.com/grbl/grbl

```
git checkout -b v0_8 origin/v0_8
make
avrdude -c arduino -P /dev/ttyUSB0 -b 57600 -p atmega328p -B 10 -U flash:w:grbl.hex:i
screen /dev/ttyUSB0 9600
$$
$0 = 72
$1 = 72
$8 = 100

G0 X10 Y10
G0 X0 Y0
```
It moves !!
`$6` to inverse axes seems to not have effect

