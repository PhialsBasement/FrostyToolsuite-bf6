# FORK CHANGES

 1. Fixed Null Reference Crashes

  - TypeLibrary.cs: Added null check in CreateObject method to return null instead of crashing when type is null
  - EbxReaderRiff.cs: Added null object handling - skips processing when objects can't be created due to missing types
  - FrostyPointerRefEditor.cs: Added null check to skip null objects when clicking the options button

  2. BF6/BFLabs Process Detection

  - SdkUpdateWindow.xaml.cs: Modified process detection to accept both "bf6event.exe" and "bflabs.exe" for Battlefield 6. When ProfileName is "bf6event", it will now also check for "bflabs" in the process name.

# KNOWN ISSUES
- Ebx to XML exporter hangs for more than necessary on some files causing extremely long export times

# FrostyToolsuite
The most advanced modding platform for games running on DICE's Frostbite game engine.

## Setup

1. Download the source code.
2. Open the solution (found under FrostyEditor) with Visual Studio 2022, and make sure the project is set to ``Release - Final`` and ``x64``. Close out of retarget window if prompted.
3. Only build the projects themselves, never the solution.

## License
The Content, Name, Code, and all assets are licensed under a Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License.
