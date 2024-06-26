# SGDeemer by https://github.com/TheHellcat/, with some modifications

### Modifications

- Hold R to use raw saving/loading features
- Bypass psp system library save console binding
	- Allows loading any Gran Turismo saves without fetching raw saves first
	- For games that bind saves to mac address as well, https://github.com/bucanero/apollo-psp is recommended, or use mac spoofing provided by most cfws
- Reduce delays so that Gran Turismo saving don't timeout
- Build against 6.61 procfw libraries
- Update SDParams->dataSize after loading raw save

### Installation

- PSP: https://www.reddit.com/r/PSP/wiki/plugins/

### Usage

- Hold R during saving to save raw `ms0:/PSP/SAVEPLAIN/<game save dir>/SDDATA.BIN` as your save data, as well as export game save keys along with the full `SceUtilitySavedataParam` struct
- Hold L+R during saving to inject modified `ms0:/PSP/SAVEPLAIN/<game save dir>/SDINFO.BIN` during saving
- Hold R during loading to load raw `ms0:/PSP/SAVEPLAIN/<game save dir>/SDDATA.BIN` as your save data
