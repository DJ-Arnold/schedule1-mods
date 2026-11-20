# schedule1-mods

Player mods for DJ's Schedule I dedicated server.

`ModUpdater.dll` goes in the game's `Plugins` folder. Each time the game starts it reads
`versions.json`, and any mod in `Mods` whose version doesn't match gets replaced with the
one in `mods/` here (checked against its sha256 first). If GitHub can't be reached the game
starts with whatever is already installed.

Turn it off with `Enabled = false` under `[ModUpdater]` in `UserData/MelonPreferences.cfg`.
