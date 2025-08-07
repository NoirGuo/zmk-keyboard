# SH1106 OLED Display Driver (External Module for Zephyr/ZMK)

This module provides an external driver for the SH1106 OLED display for use in Zephyr-based projects such as ZMK.

## Features

- I2C-based SH1106 communication
- Device tree support
- Zephyr native driver structure

## Usage

1. Add this module in your `west.yml`:

```yaml
- name: sh1106_oled
  path: modules/sh1106_oled
  url: https://github.com/your-name/sh1106_oled.git
  revision: main
```

2. Add to `ZEPHYR_EXTRA_MODULES` in `CMakeLists.txt`:

```cmake
list(APPEND ZEPHYR_EXTRA_MODULES ${CMAKE_CURRENT_SOURCE_DIR}/modules/sh1106_oled)
```

3. Enable in `prj.conf`:

```conf
CONFIG_DISPLAY=y
CONFIG_SH1106=y
```

4. Update device tree accordingly.
