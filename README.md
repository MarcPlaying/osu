# osu! [![Build status](https://ci.appveyor.com/api/projects/status/u2p01nx7l6og8buh?svg=true)](https://ci.appveyor.com/project/peppy/osu)  [![CodeFactor](https://www.codefactor.io/repository/github/ppy/osu/badge)](https://www.codefactor.io/repository/github/ppy/osu) [![dev chat](https://discordapp.com/api/guilds/188630481301012481/widget.png?style=shield)](https://discord.gg/ppy)

Rhythm is just a *click* away. The future of [osu!](https://osu.ppy.sh) and the beginning of an open era! Commonly known by the codename "osu!lazer". Pew pew.

# Fork

This fork is a little bit playing with the new osu!lazer Client! I want to add Discord Rich Presence and some other shit, all private use

# Status

This project is still heavily under development, but is in a state where users are encouraged to try it out and keep it installed alongside the stable osu! client. It will continue to evolve over the coming months and hopefully bring some new unique features to the table.

We are accepting bug reports (please report with as much detail as possible). Feature requests are welcome as long as you read and understand the contribution guidelines listed below.

# Requirements

- A desktop platform with the [.NET Core SDK 2.1](https://www.microsoft.com/net/learn/get-started) or higher installed.
- When working with the codebase, we recommend using an IDE with intellisense and syntax highlighting, such as [Visual Studio Community Edition](https://www.visualstudio.com/) (Windows), [Visual Studio Code](https://code.visualstudio.com/) (with the C# plugin installed) or [Jetbrains Rider](https://www.jetbrains.com/rider/) (commercial).

# Building and running

If you are not interested in developing the game, please head over to the [releases](https://github.com/ppy/osu/releases) to download a precompiled build with automatic updating enabled (download and run the install executable for your platform).

Clone the repository including submodules

`git clone --recurse-submodules https://github.com/MarcPlaying/osu`

Build and run

- Using Visual Studio 2017, Rider or Visual Studio Code (configurations are included)
- From command line using `dotnet run --project osu.Desktop`. When building for non-development purposes, add `-c Release` to gain higher performance.
- To run with code analysis, instead use `powershell ./build.ps1` or `build.sh`. This is currently only supported under windows due to [resharper cli shortcomings](https://youtrack.jetbrains.com/issue/RSRP-410004). Alternative, you can install resharper or use rider to get inline support in your IDE of choice.

Note: If you run from command line under linux, you will need to prefix the output folder to your `LD_LIBRARY_PATH`. See `.vscode/launch.json` for an example

If you run into issues building you may need to restore nuget packages (commonly via `dotnet restore`). Visual Studio Code users must run `Restore` task from debug tab before attempt to build.

# Licence

The osu! client code and framework are licensed under the [MIT licence](https://opensource.org/licenses/MIT). Please see [the licence file](LICENCE) for more information. [tl;dr](https://tldrlegal.com/license/mit-license) you can do whatever you want as long as you include the original copyright and license notice in any copy of the software/source.

Please note that this *does not cover* the usage of the "osu!" or "ppy" branding in any software, resources, advertising or promotion, as this is protected by trademark law.

Please also note that game resources are covered by a separate licence. Please see the [ppy/osu-resources](https://github.com/ppy/osu-resources) repository for clarifications.
