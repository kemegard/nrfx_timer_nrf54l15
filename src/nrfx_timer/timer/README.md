# TIMER {#timer_basic}

The sample demonstrates a basic functionality of the nrfx_timer driver in the Timer mode.

## Requirements

The sample supports the following development kits:


| **Board**           | **Support** |
|---------------------|:-----------:|
| nrf54l15dk          |     Yes     |


## Overview

Application initializes the nrfx_timer driver.
The @p timer_handler() is executed after a specified time.

## Wiring

To run this sample, no special configuration is needed.
User should monitor the output from the board to check if it is as expected.

## Building and running

hal\nordic\nrfx\samples\src\nrfx_timer\timer> west build -b nrf54l15dk/nrf54l15/cpuapp --no-sysbuild --pristine
hal\nordic\nrfx\samples\src\nrfx_timer\timer> west flash

## Sample output

You should see the following output:

```
    - "Starting nrfx_timer basic example"
    - "Time to wait: 1000 ms"
    - "Timer status: enabled"
    - "Timer finished. Context passed to the handler: >Some context<"
    - "Timer finished. Context passed to the handler: >Some context<"
    - "Timer finished. Context passed to the handler: >Some context<"
    - ...
```


