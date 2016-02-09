## FreeRTOS on Linux for developing and testing

### About

* To run FreeRTOS application on Ubuntu/Linux
* Based on `Posix GCC Eclipse FreeRTOS Simulator` by William Davy.
* See http://www.freertos.org/FreeRTOS-simulator-for-Linux.html
* To support latest FreeRTOS version
* Current FreeRTOS is V8.2.3

### Environment

* Linux: Ubuntu 14.04 32bit
* Tools: cmake, ...


### How to build

Please initialize submodules for the first time, need this only once.
```
$ git submodule update --init --recursive
```
This will fetch `FreeRTOS` (full) source files from the github.
Takes for a while. Please be patient.

Do build with
```
$ make
```

### Test programs

##### My first ApplicationTickHook sample

```
$ build/bin/linuxtest01
```
* To stop the program, press `CTRL+C`


### Informations

* With William's contribution, some changes was needed
  * [vTaskIncrementTick changed to xTaskIncrementTick](http://www.freertos.org/FreeRTOS_Support_Forum_Archive/October_2013/freertos_vTaskIncrementTick_changed_to_xTaskIncrementTick_2dcb1205j.html)
* This is an initial commit and don't know it's properly working or not
