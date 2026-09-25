# STM32CubeCLI Basic Tutorial Project

![STM32CubeCLI](https://img.shields.io/badge/STM32CubeCLI-blue)
![cube bundle manager](https://img.shields.io/badge/cube%20bundle%20manager-4c8c2b)
![cube-wrapper](https://img.shields.io/badge/cube--wrapper-6f42c1)
![bundles](https://img.shields.io/badge/bundles-007ec6)
![STM32](https://img.shields.io/badge/STM32-03234b)
![Tutorial](https://img.shields.io/badge/Tutorial-orange)

This repository provides an STM32 firmware project to accompany the **Your first project** STM32CubeCLI tutorial. Its purpose is to give the tutorial a concrete, CubeMX-generated CMake project that can be configured and built with a project-pinned toolchain.

## Project Overview

The project targets the **STM32F407VGTx** (Arm Cortex-M4) and uses:

- STM32CubeMX-generated startup, HAL, and system configuration
- CMake presets for Debug and Release builds
- STM32CubeCLI bundle manifests in `.settings/` to pin the project tools
- The GNU Arm toolchain and Ninja as the build generator

The board is configured as a custom target. This repository does not provide board-specific wiring, flashing, or debug instructions; the tutorial focuses on the STM32CubeCLI project and build workflow.

## Install STM32CubeCLI

Install STM32CubeCLI by following the [installation guide](https://docs.example.com/stm32cubecli/installation). This is a placeholder link for the forthcoming STM32CubeCLI documentation portal and will be updated when the portal is online.

## Get the Project

Clone the repository and change into its directory:

```sh
git clone https://github.com/stm32-hotspot/STM32CubeCLI-basic-tutorial.git
cd STM32CubeCLI-basic-tutorial
```

## Build

From the repository root, install the pinned project tools and build the Debug configuration:

```sh
cube bundle install --project
cube cmake --preset Debug
cube cmake --build --preset Debug
```

The build output is placed in `build/Debug/` or `build/Release/`.

## Feedback and Contributions

Please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) guide.