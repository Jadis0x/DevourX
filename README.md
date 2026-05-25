<p align="right">
  <img src="https://img.shields.io/badge/license-GPL--3.0-orange">
  <img src="https://visitor-badge.laobi.icu/badge?page_id=Jadis0x.DevourX">
  <img src="https://img.shields.io/github/downloads/Jadis0x/DevourX/total">
</p>

# DevourX
An advanced open-source C++ internal mod menu for the co-op horror game Devour.

### Features
#### Visuals & ESP
* Fullbright
* ESP
* Unlimited UV Light & Color Customizer

#### Gameplay
* Speed Hacks
* Fly Mode
* Instant win
* Item Spawner
* Disable Long Interactions
* Unlock All Doors/Robes
* Auto-Calm (Automatically calms Azazel when nearby.)
* Play as Azazel
* Live Chat Translator (via Google API)

#### Lobby & Steam
* Force Start Lobbies
* Bypass Player Limits
* Change Room Name
* SteamID & Name Hook Spoofing
* EXP modifier
* Walk In Lobby

### Requirements
* Windows 10/11 64-bit
* A legitimate copy of Devour installed via Steam or another supported platform
* Microsoft Visual C++ Redistributable (x64) installed [Download](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/)


### Showcase
<p align="center">
  <img src="img/Screenshot.png" width="100%">
</p>

<p align="center">
  <img src="img/Screenshot2.jpg" width="32%">
  <img src="img/Screenshot4.png" width="32%">
  <img src="img/Screenshot3.jpg" width="32%">
</p>
<p align="left">
  <strong>Controlling Azazel:</strong><br>
  <a href="https://www.youtube.com/watch?v=EcVWj-jcS3I">
    <img src="https://img.youtube.com/vi/EcVWj-jcS3I/0.jpg" alt="DevourX Video" width="90%">
  </a>
</p>

### Quick Start Installation

#### 1. Download the files
Get the latest release from this repository's [Releases](https://github.com/jadis0x/DevourX/releases) section.

The package now includes:
* version.dll
  - Core internal library.
* localization/
  - Folder containing all language JSON files.

#### 2. Locate your Devour installation folder
 - Default Steam path (might differ):
```
C:\Program Files (x86)\Steam\steamapps\common\Devour
```

#### 3. Copy all files
 - Extract everything into the main game directory, the same folder as Devour.exe

#### 4. Launch the game
 - Start Devour normally through Steam or a shortcut.
 - The game will automatically detect and load DevourX.

##### 5. Activate the menu
 - Once in-game, press `TAB` key to open or close the DevourX menu.

### Language Support
DevourX includes menu text in several languages:

- English (`en-US`)
- Turkish (`tr-TR`)
- Spanish (`es-ES`)
- German (`de-DE`)
- French (`fr-FR`)
- Korean (`ko-KR`)
- Simplified Chinese (`zh-CN`)
- Ukrainian (`uk-UA`)
- Russian (`ru-RU`)

The game asks for your preferred language the first time it runs. 

### Add another language
1. Copy `localization/en-US.json` (or the closest file) and rename it with your locale, for example `localization/es-ES.json`.
2. Translate the values, but leave the JSON keys and any placeholders like `%s` or `%d` unchanged.
3. Add your language name to the `languages` section at the top of the file so it shows up in the menu.
4. (Optional) Set it as default in `localization/config.json` while testing.

When you are done, send the new JSON file in a pull request.

### Disclaimer
* Use responsibly. Avoid disrupting public lobbies.
* This project is for educational/research purposes.

### Troubleshooting
- **Menu does not appear:** Make sure that `version.dll` is located in the same folder as `Devour.exe`.
Sometimes, Windows Defender or other antivirus programs may automatically quarantine or block `version.dll`, marking it as a potential threat.
If this happens, restore the file from quarantine and add it to your antivirus exception list before launching the game.

### Uninstalling
1. Close Devour.
2. Delete the `version.dll`.
