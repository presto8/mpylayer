# Features #

  * Dynamic commands loading.
  * Nice, descriptive error messages
  * Attribute boundary checks
  * Asynchronous operation by using select.


# Code example #

## Pythonic access to attributes and methods ##
```
mp = mpylayer.MPlayerControl()
mp.loadfile('/path/to/some_music.mp3')
mp.pause()
print mp.filename
# result: some_music.mp3
print mp.length # in seconds
# result: 234.0
print mp.time_pos
# result: 2.7766540000000002
mp.percent_pos = 50 # move to 50% of the file.
print mp.mute
# result: False
mp.mute = True # mutes output
```

Check AvailableCommandsAndProperties to see all methods/properties available.

## Good error messages: ##
```
mp.loadfile()
Traceback (most recent call last):
...
TypeError: loadfile takes ['String', '[Integer]'] arguments - String not given in ()

mp.volume = 110
Traceback (most recent call last):
...
ValueError: volume value can't be more than 100.0
```

## Descriptive doc strings ##
```
# for properties:
print type(mp).volume.__doc__
# volume  (float)
# [min: 0.0] [max: 100.0]
# change volume

# for methods:
print mp.loadlist.__doc__
# loadlist(String, [Integer])
```