# mutant_synth
Mutant Mozzi Synth with Arduino Uno, same as: [Meebleeps Mutant Mozzi Synth](https://github.com/Meebleeps/MeeBleeps-Mutant-Synth) but with an Arduino Uno
instead of Arduino Nano.

## 1 - Dependencies: 

1. [Arduino IDE](https://www.arduino.cc/en/software) (v2.0.4).
2. [Mozzi library](https://github.com/sensorium/Mozzi), follow [installation instructions](https://github.com/sensorium/Mozzi#installation).


## 2 - How to run

1. Connect the components (diagram in progress).
2. Connect Arduino Uno to USB port.
3. From the arduino IDE open the file `MutantMozziSynth/MutantMozziSynth.ino`
4. Select board then presss Upload, then after a few seconds the circuit should be ready to run. 

## 3 - Troubleshooting

### 3.1 Error: can't open device

The full error message looks like this:

```
"avrdude: ser_open(): can't open device "/dev/ttyACM0": Permission denied"
```

Solution:

Confirm that the device is available: 

```
ls /dev/ttyACM0
```

Then give permissions to read/write:

```
sudo chmod a+rw /dev/ttyACM0
```
