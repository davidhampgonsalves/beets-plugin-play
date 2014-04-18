beets-plugin-play
=================

Beets plugin that sends track query results to a music player as a playlist.

## Usage
beet play query

## Configuration
To setup the Play plugin you need to add a configurarion section as shown bellow.

```YAML
play:
    command: /Applications/VLC.app/Contents/MacOS/VLC
```

the command attribute should point to the player of your choice with any arguments required to handle a path to a m3u playlist which the plugin will append. The above example is for OSX.

You can optionally set a debug attribute to help with setting up your command attribute.
```YAML
play:
    command: cvlc
    debug: true
```

## Options
-a, --album - search by album and load album folders rather then individual tracks

## Install
this plugin can be placed inside the plugings directory of beets and configured as described above.
~/beets/beetsplug/play.py

or 

see: http://beets.readthedocs.org/en/latest/plugins/#other-plugins