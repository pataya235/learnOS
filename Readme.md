# learnOS

Based on the [Zephyr Project](https://github.com/zephyrproject-rtos/zephyr) to learn about firmware development for resource constrained devices. The Zephyr Project is a scalable real-time operating system (RTOS) supporting multiple hardware architectures, optimized for resource constrained devices, and built with security in mind.

## Prerequisites

* [CMake](https://cmake.org/)
* [Python](https://www.python.org/)
* [Devicetree compiler](https://www.devicetree.org/)
* [Host tools](https://docs.zephyrproject.org/latest/develop/getting_started/index.html#get-zephyr-and-install-python-dependencies)
* [Zephyr SDK](https://docs.zephyrproject.org/latest/develop/toolchains/zephyr_sdk.html#toolchain-zephyr-sdk)

## Usage

### Find supported boards

* /zephyr/boards/

### Find available applications

* /applications/
* /zephyr/samples/

### Build and Flash

Use [west tool](https://docs.zephyrproject.org/latest/develop/west/index.html) to trigger builds for target devices

* west build -p always -b *[board-name]* *[application-name]*

Flash device connected on serial port

* west flash
