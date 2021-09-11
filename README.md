# J4RVIS Manual

J4RVISbot is an extensible Twitch bot offering streamers access to various useful commands.

## Plugins

Various related commands and functionality are organized into plugins.  Plugins can be enabled and disabled as the streamer pleases.

### Automatic Shoutout Plugin

The Automatic Shoutout Plugin will automatically shoutout streamers visiting the channel.

#### Commands
* `!so <streamer>` This command adds a streamer to the automatic shoutout list.  It is intentially the same as the method used shoutout streamers. 
* `!solist` Lists out the streamers in the automatic shoutout list.
* `!sotest <streamer>` Sends a test shoutout message.
* `!somsg` Shows the current shoutout message.
* `!somsg <message>` Sets the current shoutout message.
   - `$name` The streamer's name.
   - `$namelower` The streamer's name in lower case.
   - `$game` The last game the streamer has played.
* `!sodelay` Show the current delay set in seconds.  Automatic shoutouts can be delayed so that mods have a chance to personally shoutout a streamer.  If a mod sends the shoutout before the automatic shoutout is sent, then the automatic shoutout will be canceled.
* `!sodelay <seconds>` Sets the delay value in seconds.  Values must be in the range of 0 to 60.
* `!sointerval`
* `!sointerval`
* `!soenable`
* `!sodisable`
* `!sosettings`
