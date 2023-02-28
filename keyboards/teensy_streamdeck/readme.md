# teensy_streamdeck

![teensy_streamdeck](imgur.com image replace me!)

*A short description of the keyboard/project*

* Keyboard Maintainer: [Fabian Gietzen](https://github.com/Fabian Gietzen)
* Hardware Supported: *The PCBs, controllers supported*
* Hardware Availability: *Links to where you can find this hardware*

Make example for this keyboard (after setting up your build environment):

    make teensy_streamdeck:default

Flashing example for this keyboard:

    make teensy_streamdeck:default:flash

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

Enter the bootloader in 3 ways:

* **Bootmagic reset**: Hold down the key at (0,0) in the matrix (usually the top left key or Escape) and plug in the keyboard
* **Physical reset button**: Briefly press the button on the back of the PCB - some may have pads you must short instead
* **Keycode in layout**: Press the key mapped to `QK_BOOT` if it is available

## Default Layout

| <!-- --> | <!-- --> | <!-- --> | <!-- --> |
| --- | --- | --- | --- |
| F19 | F17 | F15 | F13 |
| F20 | F18 | F16 | F14 |

## Media Layout

| <!-- --> | <!-- --> | <!-- --> | <!-- --> |
| --- | --- | --- | --- |
| Mute | VolDown | VolUp | F13 |
| Play | Prev | Next | F14 |

## Docker

### Build
```sh
util/docker_build.sh teensy_streamdeck:<layout>
```

### Build and Flash
```sh
util/docker_build.sh teensy_streamdeck:<layout>:flash
```
