Datacenter Operating system
===

### Building

- On Debian systems, run `scripts/setup/debian.sh` to install prerequisites.
- Make a directory for the build. We suggest `$DATACENTEROS/build/debug` or `$DATACENTEROS/build/release`.
- Run CMake from the build directory, passing the source directory in as an argument.
- Set the `CMAKE_BUILD_TYPE` variable to `Release` if you want an optimized build? You can do this with the CLI (`ccmake`) or the GUI (`cmake-gui`).
- Run `make` from the build directory.

## Cleaning

- You can clean the build by deleting the build directory and starting over.
- Run `scripts/build/clean.sh` to thouroughly clean the repository. Be warned that this will delete any untracked files that you have not yet staged.

### Notes

[//]: # (todo: does the following still apply?)
If using Mellanox ConnectX-4 NICS, DPDK needs to be compiled
with the CONFIG_RTE_LIBRTE_MLX5_PMD=y in config/common_base
