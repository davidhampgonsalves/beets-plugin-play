beets-plugin-play
=================

Beets plugin that sends track query results to a music player as a playlist.

## Usage
beet play query

## Configuration
By default the play command will use your system default application for m3u files. 

To override this you can configure the command attribute in your beets config.yaml.

```YAML
play:
    command: /Applications/VLC.app/Contents/MacOS/VLC
```

The command attribute should point to the player of your choice with any arguments required to handle a path to a m3u playlist which the plugin will append. The above example is for VLC on OSX.

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