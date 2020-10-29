# Mapvote with Previews
My modified version of mapvote, which enables map previews on the vote screen. This is based off of [tyrantelf's build of MapVote](https://github.com/tyrantelf/gmod-mapvote), originally created by [Willox.](https://github.com/willox/) The latest archive of the original thread can be found [here.](https://web.archive.org/web/20160607103800/https://facepunch.com/showthread.php?t=1268353)

It uses DHTML panels to load images from a folder hosted on the internet, so users don't need to download any bloat. This addon is pure lua.

<img src="assets/demo.gif">

See it in action on my TTT server, [func.zone](https://func.zone/ttt/).

# Configuring previews
⚠️ **Make sure to delete your old mapvote configuration;** this addon will generate a new one.

1) In your config, enable previews by setting `Previews.Enabled` to `true`.

2) Host a folder somewhere that has *direct* links of map preview images you want to display on the mapvote screen. Change `Previews.DBURL` to this folders URL.

3) Set `Previews.ImageExtension` to the image extension. Note that The images must be all of the same format. They must be browser friendly; .vtf images will NOT work.

And you're done! If the image exists, it will preview under the map vote selection.

One more configuration option;
- `Preview.InitializeWithCurrentMap`: Start the mapvote with a screenshot of the map you're currently on

