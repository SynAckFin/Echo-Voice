# Echo-Voice

This repository contains the YAML files and the design files (arriving soon) necessary for converting a 2<sup>nd</sup> Generation Amazon Echo to a Home Assistant Voice Assistant.

This is a non-destructive hardware hack that involves replacing one of the PCB's inside the Echo with a custom made control board. The Echo can always be reverted back to working with Amazon provided no accidental damage occurred when the boards were swapped.

At the present moment this repository does not have any firmware images.

## YAML Files

### ``Echo-XC56PY.yaml``

The ``XC56PY`` is the model number of the 2<sup>nd</sup> Generation Echo.

This file includes the YAML file from [Home Assistant Voice Preview Edition](https://github.com/esphome/home-assistant-voice-pe), as a package, and modifies the GPIO and platform settings to match the Echo's and the custom control board's architecture. As a result the Echo has the same behaviour as the Home Assistant Voice, including sound and lighting effects.

This YAML file will not compile on its own, it needs to be included by another YAML file that has the wifi and other settings. Two example YAML files are included.

### ``Example-001.yaml``

This is a basic example that contains the device name and network credentials. This is what is being used to generate the firmware for the prototype control boards.

### ``Example-002.yaml``

This is slightly more advanced and remaps all the GPIOs. This is what is being used to generate the firmware for my development board.

## Coffee

Building prototype PCB's isn't cheap so if you would like to support this project you can [buy me a coffee](https://buymeacoffee.com/trsanders).
