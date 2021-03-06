# Twitch Viewer Count
A CLR Browser URL that displays channel viewer count for embedding within an OBS scene.

# Requirements
- [Open Broadcaster Software (OBS)](https://obsproject.com/)
- [NightDev's CLR Browser 4 Repack](http://cdn.nightdev.com/clrbrowser4_repack.zip)

# Usage

There are several variables you can append to the URL:
```
channel=TwitchChannelName // your twitch channel name
size=100 // font size
color=hotpink // font color
family=Tahoma // font family
seconds=10 // interval update in seconds
style=anime // custom style
debug=123456 // custom debug values for test (Max is 999999)
```
- Style it the way you like.
- Selecting "anime" for the style overrides all other style settings.
- If you do not specify, default values are Black font color, 90px font size, Tahoma font family, 10 second intervals, no style
- .gif files go into the same directory as viewercount.php
- Debug will only work when the Twitch API returns a non-null value for 'stream' data.  Basically, the stream must be live and broadcasting.

# Example:
```
viewercount.php?channel=monstercat&size=100&color=hotpink&family=Tahoma&seconds=15
viewercount.php?channel=monstercat&style=anime&seconds=5
viewercount.php?channel=monstercat&style=touhou
viewercount.php?channel=monstercat&style=anime&debug=123123
```
# Live Example

- [Example 1](http://www.intechnicolor.net/twitch/viewercount.php?channel=monstercat&size=100&color=hotpink&family=Tahoma&seconds=15)
- [Example 2](http://www.intechnicolor.net/twitch/viewercount.php?channel=monstercat&style=anime&seconds=5)
- [Example 3](http://www.intechnicolor.net/twitch/viewercount.php?channel=monstercat&style=touhou)
- [Example 4](http://www.intechnicolor.net/twitch/viewercount.php?channel=monstercat&style=anime&debug=123123)
