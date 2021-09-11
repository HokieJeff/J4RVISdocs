# J4RVIS Manual

J4RVISbot is an extensible Twitch bot offering streamers access to various useful commands.

## Plugins

Various related commands and functionality are organized into plugins.  Each plugin can be enabled and disabled independently of each other.

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
* `!sodelay` Shows the current delay value in seconds.  Automatic shoutouts can be delayed so that mods have a chance to personally shoutout a streamer.  If a mod sends a shoutout before the automatic shoutout is sent, due to the delay, then the automatic shoutout will be canceled.
* `!sodelay <seconds>` Sets the delay value in seconds.  Values must be in the range of 0 to 60 seconds.  The default delay is 20 seconds.
* `!sointerval` Shows the current shoutout interval in minutes.  The interval controls the amount of time that needs to have elapsed since a streamer's last shoutout, before the streamer is eligible to receive an automatic shoutout.
* `!sointerval <minutes>` Sets the shoutout interval in minutes. The minimum value is 1 minute, and the maximum value is 1,440 minutes (24 hours).  The default interval is 3 hours.
* `!soenable` Enables the Automatic Shoutout feature.
* `!sodisable` Disables the Automatic Shoutout feature.
* `!sosettings` Shows the status of the Automatic Shoutout feature (enabled/disabled) and reports the delay value and the interval value.

### Search Plugin

The Search Plugin allows users to search through the broadcaster's clips, returning the best match.

#### Commands
* `!search <search term>` Searches through the broadcaster's clips, returning the best match.  The search currently searches through roughly 1000 clips.  It works pretty well if you know the title of the clip you're searching for, but it's hit or miss for broad general searches.
