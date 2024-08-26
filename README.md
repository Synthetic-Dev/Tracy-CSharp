# Tracy CSharp for Godot

![](Header.png)

> This is a fork of [Tracy-CSharp](https://github.com/clibequilibrium/Tracy-CSharp) made to work with .NET 6 and Godot

C# bindings for https://github.com/wolfpld/tracy with native dynamic link libraries based on [`imgui-cs`](https://github.com/bottlenoselabs/imgui-cs).

## How to use

## Get it from [NuGet](https://www.nuget.org/packages/tracy-csharp-godot)

```bash
dotnet add package tracy-csharp-godot --version 0.10.0.2
```

## From source

### Installing `C2CS`

`C2CS` is distributed as a NuGet tool. To get started, the .NET 7 (or later) software development kit (SDK) is required.

#### Latest release of `C2CS`

```bash
dotnet tool install bottlenoselabs.c2cs.tool --global
```

1. Download and install [.NET 7 or later](https://dotnet.microsoft.com/download).
2. Fork the repository using GitHub or clone the repository manually with submodules: `git clone --recurse-submodules https://github.com/Synthetic-Dev/tracy-csharp-godot`.
3. Build the native library by running `library.sh`. To execute `.sh` scripts on Windows, use Git Bash which can be installed with Git itself: https://git-scm.com/download/win. The `library.sh` script requires that CMake is installed and in your path.
4. Locate the sample of the C# project: `./src/cs/samples/HelloWorld/HelloWorld.csproj`.

## Developers: Documentation

For more information on how C# bindings work, see [`C2CS`](https://github.com/lithiumtoast/c2cs), the tool that generates the bindings for `Tracy` and other C libraries.

To learn how to use `Tracy`, check out the [official readme](https://github.com/wolfpld/tracy).

All of the C# bindings can be found in [the generated file `PInvoke.gen.cs`](https://github.com/Synthetic-Dev/tracy-csharp-godot/blob/main/src/cs/production/Tracy/Generated/PInvoke.gen.cs)

## License

`Tracy-CSharp` is licensed under the MIT License (`MIT`) - see the [LICENSE file](LICENSE) for details.

`Tracy` itself is licensed under BSD license (`BSD`) - see https://github.com/wolfpld/tracy/blob/master/LICENSE for more details.
