Please report bugs on [GitHub](https://github.com/Henner4746/FlightAssistant/issues). This is an unofficial fork, so please don't report its problems to the original FlightAssistant project.

## Changes in 3.3.0

- Added support for Minecraft 26.1 and 26.1.2
- The 26.1 and 26.1.2 builds use the matching versions of Fabric API, YetAnotherConfigLib, Architectury API, Mod Menu and Do a Barrel Roll
- Adapted the HUD, screens and widgets to the `GuiGraphicsExtractor` pipeline introduced in 26.1
- Kept 26.1's GLFW key handling and TinyFD flight plan dialogs, which were only replaced by SDL in 26.3
- Added Modrinth's Maven repository to resolve Do a Barrel Roll's 26.1 runtime dependencies
- The 26.1 and 26.1.2 builds render screens through the framework's background extraction, avoiding the double-blur crash fixed for 26.2

## Changes in 3.2.0

- Added support for Minecraft 26.3
- Fixed a crash when opening the FlightAssistant setup screen or its menus while in a world ("Can only blur once per frame")
- The 26.2 version is now built against the real 26.2 versions of Fabric API, YetAnotherConfigLib and Architectury API
- Declared all required dependencies (YetAnotherConfigLib, Architectury API) so launchers install them automatically

### Minecraft 26.3 specifics

- Default key bindings were adapted to the new input system in 26.3 (Numpad Enter, Numpad 0, Numpad ., arrow keys, Caps Lock, Left Alt)
- Saving and loading flight plans now uses the system file dialog provided by 26.3
