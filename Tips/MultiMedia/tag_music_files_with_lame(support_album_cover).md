# Lame Options

### Usage :
`lame [options] <infile> [outfile]`

### Convert :
`lame -V2 input.wav output.mp3`

### Add album art :
`lame --ti AlbumArt.jpg music.mp3`

### ID3 tag options :

| Option                | Description |
|-----------------------|-------------|
|`--tt <title>`         | audio/song title (max 30 chars for version 1 tag) |
|`--ta <artist>`        | audio/song artist (max 30 chars for version 1 tag) |
|`--tl <album>`         | audio/song album (max 30 chars for version 1 tag) |
|`--ty <year>`          | audio/song year of issue (1 to 9999) |
|`--tc <comment>`       | user-defined text (max 30 chars for v1 tag, 28 for v1.1) |
|`--tn <track[/total]>` | audio/song track number and (optionally) the total number of tracks on the original recording. (track and total each 1 to 255.|
|`--tg <genre>`         | audio/song genre (name or number in list) |
|`--ti <file>`          | audio/song albumArt (jpeg/png/gif file, v2.3 tag) |
|`--tv <id=value>`      | user-defined frame specified by id and value (v2.3 tag) |
|`--add-id3v2`          | force addition of version 2 tag |
|`--id3v1-only`         | add only a version 1 tag |
|`--id3v2-only`         | add only a version 2 tag |
|`--id3v2-utf16`        | add following options in unicode text encoding |
|`--id3v2-latin1`       | add following options in latin-1 text encoding |
|`--space-id3v1`        | pad version 1 tag with spaces instead of nulls |
|`--pad-id3v2`          | same as '--pad-id3v2-size 128' |
|`--pad-id3v2-size`     | <value> adds version 2 tag, pad with extra <value> bytes |
|`--genre-list`         | print alphabetically sorted ID3 genre list and exit |   |`--ignore-tag-errors`  | ignore errors in values passed for tags |


