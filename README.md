## C&C Tiberian Dawn and Red Alert Map Editor

This is a fork of Rampastrings enhanced version of the C&C Tiberian Dawn and Red Alert Map Editor, based on the source code released by Electronic Arts.
Rampastrings project was to improve the usability and convenience of the map editor.

This fork is to add support for creating 128x128 maps in TD.

### Current features

* Downsized menu graphics by an user-configurable factor so you can see more placeable object types at once on sub-4K monitors
* Improved zoom levels
* Fixed a couple of crashes
* Made tool windows remember their previous position, size and other settings upon closing and re-opening them
* Replaced drop-downs with list boxes in object type selection dialogs to allow switching between objects with fewer clicks 
* Can now edit/create TD maps in 128x128 size using the Sole Survivor binary format.

### Installation

To install, simply download a compiled build from the [Releases section of this repository](https://github.com/screamingchicken/CnCTDRAMapEditor/releases)
and unzip the build into a new directory.
**Do not overwrite the original map editor that comes with the C&C Remastered Collection**. The map editor will ask for your game
directory on first launch and then load all assets from the specified directory.

### Usage
* Comments detailing how the Sole Survivor binary format works have been embedded in the code if anyone is interested.
* Normal sized 64x64 maps will still use the original TD binary format.
* 128x128 maps will use a key in their ini file which sets "Version=1"

### Compiling this or Rampastrings code
1) VS2017 needs JSON, Pfim and System.ValueTuple packages
2) It possibly needs the NETStandard package
3) It needs the .csproj file modified to add the following line alongside the References:
```
<Reference Include="netstandard" />
```
4) The EA/Petro code has no comments, unless they're really hidden somehow.



