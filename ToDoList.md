# TODO #

  * add mencoder support. I want to be able do this:
```
>>> me = mpylayer.MEncoderControl()
>>> me.input="xpto.avi"
>>> me.output="abc.mpeg"
>>> me.ovc("lavc")
>>> me.ovc.vbitrate=200
>>> me() # runs encoder
```
  * add SSH support. So you can control remote mplayers.