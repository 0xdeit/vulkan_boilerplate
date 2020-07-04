# vulkan_boilerplate
Simple Vulkan (C++ 17) Boilerplate based on the Vulkan Tutorial

## Works on
- Linux 
	> Tested on Fedora 32 (Meson [0.54.3] / Ninja [1.10]) 
- Windows
	> Tested on Windows 10 20H2 (Visual Studio 2019 [16.6.3] and vcpkg [2020.02.04-nohash])

## Dependencies:
- GLFW3 ([GLFW](https://www.glfw.org/))
- Vulkan ([LunarG](https://vulkan.lunarg.com/sdk/home))

## Getting Started (Linux)
- Recommended: Use your system's package manager to install dependencies
  - TODO: List packages per distro
- In project's root directory, run `meson setup build_dir`. 
This step will set the compiler from the system's default, `gcc` on most Linux distributions.
- To build the project run either `meson compile -C build_dir` or `ninja -C build_dir`
- Go to `build_dir` and run the executable `vulkan_boilerplate`
- You should see a blank window with the title `Vulkan Boilerplate`

> Optional: Use helper scripts `setup_debug_clang.sh` and `run_debug.sh` instead of the previous workflow.  
> Default compiler will be Clang++ and build directory is `debug_clang`.

## Getting Started (Windows)
Project is configured to use `vcpkg` to handle the dependencies.
- Recommended: Install vcpkg ([Github](https://github.com/microsoft/vcpkg))
  - Install GLFW3 x64 `vcpkg install glfw3:x64-windows`
  - Install Vulkan SDK `vcpkg install vulkan:x64-windows`
- Optional: Manage the dependencies manually, this will require you to modify the project's settings.
Reference the [Vulkan Tutorial](https://vulkan-tutorial.com/) for this: [Development Environment](https://vulkan-tutorial.com/Development_environment)

> Make sure that the environment variable VULKAN_SDK exists and points to the Vulkan SDK install directory.

- Open the solution `VulkanBoilerplate\VulkanBoilerplate.sln`
- Run the project
- You should see a blank window with the title `Vulkan Boilerplate`

