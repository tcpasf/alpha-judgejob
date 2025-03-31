# Alpha Judge Job

A comprehensive judge job script for QBCore Framework, providing essential tools and functionality for judges in your FiveM server.

## Features

- **Judge Hammer**: Use the gavel to call for order in the courtroom with custom sound effects
- **Microphone System**: Enhanced voice projection in the courtroom
- **Boss Menu**: Manage your judge department with employee management and finances
- **Clothing Menu**: Quick access to judge robes and attire
- **Vehicle Spawn**: Dedicated vehicle spawner for judges
- **Complaint System**: Citizens can file complaints against officers, which judges can review
- **Court Messaging**: Broadcast court announcements to everyone in the courtroom
- **PMA-Voice Integration**: Voice amplification for judges when using the microphone

## Dependencies

- [qb-core](https://github.com/qbcore-framework/qb-core)
- [qb-target](https://github.com/qbcore-framework/qb-target)
- [qb-menu](https://github.com/qbcore-framework/qb-menu)
- [qb-clothing](https://github.com/qbcore-framework/qb-clothing)
- [qb-management](https://github.com/qbcore-framework/qb-management)
- [pma-voice](https://github.com/AvarianKnight/pma-voice)

## Installation

1. Download the resource
2. Place it in your server's resource folder
3. Add `ensure alpha-judgejob` to your server.cfg
4. Configure the settings in `config/alpha_config.lua` to match your server's needs
5. Restart your server

## Configuration

The script is highly configurable through the `config/alpha_config.lua` file:

```lua
Config = {}

Config.RequiredJob = "police" -- Job required to use judge features

-- Locations
Config.JudgePosition = vector3(451.43, -1091.17, 30.33)
Config.BossMenuPosition = vector3(446.72, -1103.55, 29.91)
Config.ClothingPosition = vector3(444.62, -1100.89, 30.24)
Config.CarSpawnPosition = vector4(402.62, -1085.02, 29.31, 355.71)
Config.CarSpawnPedPosition = vector4(404.41, -1083.0, 29.41, 93.44)
Config.ComplaintPedPosition = vector4(433.79, -1092.01, 30.06, 90.0)
Config.CourtRoomCenter = vector3(452.26, -1093.11, 30.53)
Config.ComplaintReviewPosition = vector3(446.43, -1103.01, 29.9)

-- Peds
Config.CarSpawnPed = "s_m_y_cop_01"
Config.ComplaintPedModel = "a_f_y_business_02"

-- Sound Settings
Config.HammerSoundFile = "sounds/hammer.ogg"
Config.MicBoostMultiplier = 1.5
Config.PmaVoiceBoost = 2.0
Config.SoundRadius = 30.0

-- Court Messages
Config.CourtMessages = {
    "Order in the court!",
    "Silence in the courtroom!",
    "The court is now in session!",
    "All rise for the honorable judge!",
    "This court is now in order!"
}

-- Props
Config.MicProp = "prop_microphone_02"

-- Vehicles
Config.Vehicles = {
    "adder",
    "police",
    "ambulance",
    "baller",
    "cognoscenti",
    "schafter2",
    "stretch"
}
```

## Usage

### Judge Hammer
Approach the judge's bench and use the target option to use the hammer. This will play a sound and send a court message to everyone in the courtroom.

### Microphone
Use the target option to equip/unequip the microphone. While holding the microphone, your voice will be amplified in the courtroom.

### Boss Menu
Access the boss menu at the designated location to manage employees and finances for the judge department.

### Clothing Menu
Access the clothing menu at the designated location to quickly change into judge attire.

### Vehicle Spawn
Speak with the vehicle spawn NPC to access the judge's vehicle options.

### Complaint System
Citizens can file complaints at the designated NPC. Judges can review these complaints at the complaint review position.

## Commands

- None currently implemented

## Credits

Developed by AlphaDev from RedEye Team

## License

All rights reserved. This resource is provided for use on authorized servers only. Redistribution or modification without explicit permission is prohibited.

© 2023 RedEye Team
