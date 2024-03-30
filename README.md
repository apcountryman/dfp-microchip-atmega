# dfp-microchip-atmega

Microchip Technology Inc. ATmega series Device Family Pack (DFP) packaged as a Git
repository.
Source: [Microchip Packs Repository](https://packs.download.microchip.com/).

## Obtaining the Source Code

HTTPS:
```shell
git clone https://github.com/apcountryman/dfp-microchip-atmega.git
```
SSH:
```shell
git clone git@github.com:apcountryman/dfp-microchip-atmega.git
```

## Usage

The contents of the DFP can be found in the [`dfp/`](dfp) directory of this repository.

```shell
git submodule add https://github.com/apcountryman/dfp-microchip-atmega.git
```
```CMake
add_compile_options(
    -mmcu=atmega4809
    -B "${CMAKE_CURRENT_SOURCE_DIR}/dfp-microchip-atmega/gcc/dev/atmega4809"
    )

include_directories( SYSTEM
    "${CMAKE_CURRENT_SOURCE_DIR}/dfp-microchip-atmega/include"
    )
```

## License

Microchip Technology Inc. releases the ATmega series DFP under the Apache License, Version
2.0.
For more information, see the [`EULA`](EULA) and [`LICENSE`](LICENSE) files in this
repository.
