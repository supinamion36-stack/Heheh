# Roblox game

Ponytail mode is on by default for all work in this project: load the `ponytail` skill (level `full`) at the start of every session and follow it until the user says "stop ponytail" or "normal mode" or switches level with `/ponytail lite|ultra`.

Roblox-specific limits on being lazy (never cut these):
- The server validates everything a client sends through RemoteEvents/RemoteFunctions; never trust the client.
- DataStore calls stay wrapped in `pcall` with retry; never risk losing player data.
- Prefer built-in Roblox services (TweenService, CollectionService, ProfileService only if already used) over new modules.
