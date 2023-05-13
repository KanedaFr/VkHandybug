# VkHandybug

Debugger for the Atari Lynx emulator [Handy](https://handy.sourceforge.net/).

Based on ImGui, GLFW/Vulkan, reasonably cross platform (Linux - GCC 12.1, Windows - Visual Studio 2022).

![](/assets/screen1.jpg)

# Binaries
Latest Windows binaries can currently be found on the [releases](https://github.com/LLeny/VkHandybug/releases) page.

# Usage
You will first need to set the Lynx ROM image path, please use the ```MAIN -> Settings...``` menu to do so.

To load symbols create a file with the same name as the cart but with the .lbl extension.
The *lbl* file can be a Vice label file (generated by [cl65](https://cc65.github.io/doc/cl65.html) -Ln option) or simply be a list of "addr label".

```
  0034 here
  4ADE andhere
```

# Building
## Dependencies

- [Vulkan SDK](https://www.lunarg.com/vulkan-sdk/), please refer to your system's [vulkan "Getting Started"](https://www.lunarg.com/vulkan-sdk/) page for installation.
- [CMake](https://cmake.org/) is required as the build files generator.

## Compiling
### Linux
 ```
 git clone https://github.com/LLeny/VkHandybug.git
 cd VkHandybug
 mkdir build
 cd build
 cmake -DCMAKE_BUILD_TYPE=Release ..
 cmake --build .
 ```
 
 The binary should be created in the folder ```./bin```

 # Dependencies
 - [cereal](https://uscilab.github.io/cereal/)
 - [csys](https://github.com/rmxbalanque/csys)
 - [Dear ImGui](https://github.com/ocornut/imgui)
 - [GLFW](https://www.glfw.org/)
 - [hash-library](https://create.stephan-brumme.com/hash-library/)
 - [imgui-console](https://github.com/rmxbalanque/imgui-console)
 - [ImGuiFileDialog](https://github.com/aiekick/ImGuiFileDialog)
 - [imgui_memory_editor](https://github.com/ocornut/imgui_club)
 - [miniaudio](https://miniaud.io/)
 - [vk-bootstrap](https://github.com/charles-lunarg/vk-bootstrap)
 - [Vulkan Memory Allocator](https://gpuopen.com/vulkan-memory-allocator/)
 - [Vulkan SDK](https://www.lunarg.com/vulkan-sdk/)
 - [zlib](https://github.com/madler/zlib)
 - [{fmt}](https://fmt.dev/latest/index.html)
