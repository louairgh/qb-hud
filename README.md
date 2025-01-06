# Kane-qb-hud-Nopixel-4.0-inspired (Edited Version)

This is an edited version of the original **Kane-qb-hud-Nopixel-4.0-inspired** script, inspired by the NoPixel 4.0 HUD for the **QBCore Framework**. The script provides a dynamic, feature-rich Heads-Up Display (HUD) with various elements such as health, armor, hunger, thirst, and more.

![Screenshot 2025-01-06 165111](https://github.com/user-attachments/assets/93cdcd3d-4ac2-4664-8dbd-a14944ba6ef3)

## Features

- **Customizable HUD**: Edit the layout, colors, and elements to fit your server's needs.
- **Safe Zone Integration**: The HUD automatically adjusts its display based on whether the player is in a safe zone or not.
- **Detailed Player Information**: Displays health, armor, hunger, thirst, and money with dynamic updates.
- **Enhanced UI Design**: Inspired by the popular NoPixel 4.0 HUD with additional custom modifications.
- **Flexible Configuration**: Easily configure the HUD elements using the `config.lua` file.

## Installation

1. Clone or download this repository.
2. Place the `qb-hud` folder in your server's **resources** directory.
3. Add `ensure qb-hud` to your server configuration file (`server.cfg`).
4. Configure the HUD settings in `qb-hud/config.lua` to match your server's preferences.
5. Restart your server to load the new HUD.

## Configuration

To customize the HUD, open the `config.lua` file located inside the `qb-hud` folder. Here you can:

- Adjust the positions of UI elements.
- Change color schemes for various HUD components.
- Enable or disable certain features like hunger, thirst, and money displays.
- Modify the safe zone behavior (e.g., hide HUD elements when in safe zones).

## Dependencies

- **QBCore Framework**: This script is designed to work with the QBCore framework.

## Modifications

This version includes the following modifications:
- Integrated **safe zone functionality**: The HUD automatically hides specific UI elements when the player is in a designated safe zone.
- Updated **UI layouts and animations** to improve the user experience.
- Additional **customizable options** to further personalize the HUD for your server.

## Adding New Safe Zones

To add new safe zones, you can define them in the `client.lua` file. You can create custom polygonal areas for each safe zone by specifying the coordinates.

Example of adding a new safe zone (HotelZone):

```lua
local HotelZone = PolyZone:Create({
    vector2(-371.8846130371, -855.71673583984),
    vector2(-371.57205200196, -967.6898803711),
    -- Add more coordinates for the Safe Zone shape
}, {
    name = "HotelZone",
    debugPoly = false
})
```
## Credits

- Original script by **rohKane**: [GitHub](https://github.com/rohKane)
- **NoPixel 4.0-inspired** design and layout.

## License

This script is open-source and licensed under the MIT License. You are free to modify and distribute it, but please provide appropriate credit to the original creator.
