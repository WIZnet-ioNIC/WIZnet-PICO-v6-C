# RP2040 & W6x00 Ethernet Examples

- [**Overview**](#overview)
- [**Getting Started**](#getting_started)
- [**Directory Structure**](#directory_structure)
- [**Appendix**](#appendix)
    - [**Other Examples**](#other_examples)



<a name="overview"></a>
## Overview

The RP2040, RP2350 & W6x00 ethernet examples use **W6100-EVB-Pico** and **W6100-EVB-PICO2** - ethernet I/O modules built on [**RP2040**][link-rp2040], [**RP2350**][link-rp2350] and WIZnet's [**W6100**][link-w6100] ethernet chip.

- [**W6100-EVB-Pico**][link-w6100-evb-pico]

![][link-w6100-evb-pico_main]

- [**W6100-EVB-Pico2**][link-w6100-evb-pico2]

![][link-w6100-evb-pico2_main]



<a name="getting_started"></a>
## Getting Started

Please refer to [**Getting Started**][link-getting_started] for how to configure development environment or examples usage.

# Setup board

1. Setup the board in '**CMakeLists.txt**' in '**WIZnet-PICO-v6-C/**' directory according to the evaluation board to be used referring to the following.

- W6100-EVB-Pico
- W6100-EVB-Pico2

2. For example, when using W6100-EVB-Pico :

```cpp
# Set board
set(W6100-EVB-Pico)
```

When using W6100-EVB-Pico2 :

```cpp
# Set board
set(BOARD_NAME W6100_EVB_PICO2)
```



<a name="directory_structure"></a>
## Directory Structure

```
RP2040-v6-HAT-C
┣ examples
┃   ┣ AddressAutoConfiguration
┃   ┗ loopback
┣ libraries
┃   ┣ io6Library
┃   ┣ mbedtls
┃   ┣ pico-extras
┃   ┗ pico-sdk
┣ port
┃   ┣ io6Library
┃   ┣ mbedtls
┃   ┗ timer
┗ static
    ┣ documents
    ┗ images
```



<a name="appendix"></a>
## Appendix



<a name="other_examples"></a>
### Other Examples

- C/C++
    - [**RP2040-v6-HAT-FREERTOS-C**][link-rp2040-v6-hat-freertos-c]



<!--
Link
-->

[link-rp2040]: https://www.raspberrypi.org/products/rp2040/
[link-w6100]: https://docs.wiznet.io/Product/iEthernet/W6100/overview
[link-w6100-evb-pico]: https://docs.wiznet.io/Product/iEthernet/W6100/w6100-evb-pico
[link-w6100-evb-pico_main]: https://github.com/Wiznet/RP2040-v6-HAT-C/blob/main/static/images/w6100-evb-pico_main.png
[link-w6100-evb-pico2]: https://docs.wiznet.io/Product/iEthernet/W6100/w6100-evb-pico2
[link-w6100-evb-pico2_main]: https://docs.wiznet.io/assets/images/w6100-evb-pico2-docs-0d662aa52a0089de8d06d14d756c1e12.png
[link-getting_started]: https://github.com/Wiznet/RP2040-v6-HAT-C/blob/main/static/documents/getting_started.md
[link-rp2040-v6-hat-freertos-c]: https://github.com/Wiznet/RP2040-v6-HAT-FREERTOS-C