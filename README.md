# Jump Racer

Jump Racer is a 2018 OutRun-style pseudo-3D racing prototype written in C++14
with SFML. It projects road segments and sprites into a 1024 x 768 window and
includes music, traffic sprites, collision feedback, curves, and hills.

> Project status: historical prototype. The repository includes an old Windows
> debug build and its runtime DLLs. It is not a current packaged release.

## Run the included Windows build

Clone the repository, change to the directory that contains the executable and
its `images` folder, and run it:

```powershell
git clone https://github.com/AbrarZShahriar/jump-racer-sfml.git
cd jump-racer-sfml\bin\Debug
.\JumpRacer.exe
```

The executable is an unsigned historical binary. Build the source yourself if
you do not want to run a checked-in binary.

## Controls

- `Left` and `Right` steer.
- `Down` drives backward.
- `Tab` increases the forward speed while held.
- `Space` raises the car to simulate a jump.
- `S` lowers the camera height while held.

## Build from source

`JumpRacer.cbp` is a Code::Blocks project configured for a 64-bit MinGW GCC
7.3 toolchain, C++14, and SFML 2. The checked-in project contains old absolute
MinGW paths, so update its compiler and linker search paths for your local
installation.

Required SFML libraries are `sfml-graphics`, `sfml-audio`, `sfml-window`, and
`sfml-system`. Keep the `images` directory and required SFML/OpenAL runtime
DLLs next to the executable when you run a new build.

## License

The project source is available under the [MIT License](./LICENSE). Bundled
music, images, and third-party runtime libraries can have separate terms.
