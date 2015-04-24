# nucleo-stm32f303-blinky
ST Nucleo STM32F303RET6 Blinky Using Eclipse + GNU ARM Plugins + OpenOCD via Nucleo ST-Link

## Status

OpenOCD v0.9 works with integrated ST-Link for debugging and flashing.

### OpenOCD

* The best path forward for development work.
* Works with semi-hosting for a handy local console.
* Needs OpenOCD 0.9.0-dev-00415-g2d4ae3f or later for flashing to work.


### stlink

* Has initial support for STM32F303 high density device via [kylemanna/stlink](https://github.com/kylemanna/stlink).
* Works to flash devices pretty seemlessly via gdb.
* Doesn't appear to have any support for ARM semihosting which causes tons of IRQs if the preprocessor macro isn't disabled.
* Fall back if OpenOCD isn't working.
