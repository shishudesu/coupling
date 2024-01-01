# Coupling
Media Server for Chaos communications.
## Building Instructions
First clone the repository with its submodule dependencies using:
```bash
$ git clone --recurse-submodules https://github.com/shishudesu/coupling
```
Create a build folder and change directory:
```bash 
$ cd coupling
$ mkdir build && cd build
```
Generate build files in the build folder using the generator of your choice:
```bash
$ cmake ..
```
>I recommend using the Ninja Multi-Config Generator.
> ```bash
> $ cmake .. -G "Ninja Multi-Config"
> ```
Build the project:
```bash
$ cmake --build . 
```
> You can specify your build config if you used a Multi-Config generator
> ```bash
> $ cmake --build . --config <Config>
>```
> For `Ninja Multi-Config`, `Debug` `Release` and `RelWithDebInfo` are available.
