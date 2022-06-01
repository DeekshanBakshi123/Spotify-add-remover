

#### Important checks before installing:
0. Update Windows, update Spotify and update BlockTheSpot
1. Go to "Windows Security" -> "Virus & Threat Protection"
2. Click "Allowed threats" -> "Remove all allowed threats"

### Features:
* Blocks all banner/video/audio ads within the app
* Retains friend, vertical video and radio functionality
* Unlocks the skip function for any track

:warning: This mod is for the [**Desktop Application**](https://www.spotify.com/download/windows/) of Spotify on Windows only and **not the Microsoft Store version**.

### Installation/Update:
* Just download and run [BlockTheSpot.bat](https://raw.githack.com/mrpond/BlockTheSpot/master/BlockTheSpot.bat)  

or

#### Fully automated installation via PowerShell

```powershell
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; Invoke-Expression "& { $(Invoke-WebRequest -UseBasicParsing 'https://raw.githubusercontent.com/mrpond/BlockTheSpot/master/install.ps1') } -UninstallSpotifyStoreEdition -UpdateSpotify -RemoveAdPlaceholder"
```

#### Manual installation

1. Browse to your Spotify installation folder `%APPDATA%\Spotify`
2. Rename `chrome_elf.dll` to `chrome_elf_bak.dll`. The naming is important.
3. Download `chrome_elf.zip` from [releases](https://github.com/mrpond/BlockTheSpot/releases)
4. Unzip `chrome_elf.dll` and `config.ini` to Spotify directory. 

### Uninstall:
* Just run [uninstall.bat](https://raw.githack.com/mrpond/BlockTheSpot/master/uninstall.bat)
or
* Reinstall Spotify

### Known Issues:  
* [#150](https://github.com/mrpond/BlockTheSpot/issues/150): Can be fixed by enabling the experimental feature when using `BlockTheSpot.bat`.
* [#289](https://github.com/mrpond/BlockTheSpot/issues/289): Rare issue where audio ads may not get blocked sometimes.

