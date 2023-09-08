# JUCE CMake Plugin Template

Configurable base template for a JUCE audio plugin using CMake

## Requirements

- git 2.13+
- cmake 3.15+

## Getting Started

#### 1. Recursively clone this repo
`git clone --recurse-submodules https://github.com/tadashibashi/juce-cmake-plugin-template`

#### 2. Run customary mkdir build && cd build && cmake .. && cmake --build

## Project Structure

```text
/
├─ lib/                    # Submodule dependencies
│  ├─ JUCE/                
├─ src/                    # Plugin boilerplate code
│  ├─ PluginEditor.cpp
│  ├─ PluginEditor.h
│  ├─ PluginProcessor.cpp
│  ├─ PluginProcessor.h
├─ CMakeLists.txt          # Build configurations
├─ ReadMe.txt              # This file
```

## How to Use

- CMakeLists.txt is where you can configure the project --
project name, manufacturer, plugin type, compile defs etc.
- Add all source files to `src/` and write each in the CMakeLists.txt 
`target_sources` command.
