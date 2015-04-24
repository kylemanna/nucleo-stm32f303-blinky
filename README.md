# nucleo-stm32f303-blinky
ST Nucleo STM32F303RET6 Blinky Using Eclipse + GNU ARM Plugins + OpenOCD via Nucleo ST-Link

## Status

Kind of works in 2 different ways.

### OpenOCD

* Works with semi-hosting for a handy local console.
* Needs a patch in `stm32x_probe()` to properly detect the chip for flashing.
* Probably the best path forward for Eclipse development work.


### stlink

* Has initial support for STM32F303 high density device via [kylemanna/stlink](https://github.com/kylemanna/stlink).
* Works to flash devices pretty seemlessly via gdb.
* Doesn't appear to have any support for ARM semihosting which causes tons of IRQs if the preprocessor macro isn't disabled.
