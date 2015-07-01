# Varying commands and properties #

The mplayer commands are generated on the fly using `mplayer -input cmdlist`, since the commands available can vary on each mplayer compilation.

The list of properties is hard-coded, since I couldn't find a way to get it from mplayer itself.

# The actual list #

You can get a list by using the following code:
```
import mpylayer
mp = mpylayer.MPlayerControl()
help(mp)
```

Below is the result of running this command on my system, with a few _private_ methods manually removed.

Note that your actual list may vary, since part of it is extracted dynamically from mplayer itself.

```
Help on MPlayerControl in module mpylayer.mpylayer_control object:

class MPlayerControl(__builtin__.object)
 |  Methods defined here: 
 |  __init__(self, mplayer_path='mplayer')
 |      Starts a new mplayer process.
 |      mplayer_path is the path to mplayer, defaults to 'mplayer'.
 |  
 |  alt_src_step(self, *args, **kwds)
 |      alt_src_step(Integer)
 |  
 |  change_rectangle(self, *args, **kwds)
 |      change_rectangle(Integer, Integer)
 |  
 |  dvb_set_channel(self, *args, **kwds)
 |      dvb_set_channel(Integer, Integer)
 |  
 |  dvdnav(self, *args, **kwds)
 |      dvdnav(Integer)
 |  
 |  edl_mark(self, *args, **kwds)
 |      edl_mark()
 |  
 |  exit(self, *args, **kwds)
 |      exit()
 |  
 |  file_filter(self, *args, **kwds)
 |      file_filter(Integer)
 |  
 |  forced_subs_only(self, *args, **kwds)
 |      forced_subs_only([Integer])
 |  
 |  frame_drop(self, *args, **kwds)
 |      frame_drop([Integer])
 |  
 |  frame_step(self, *args, **kwds)
 |      frame_step()
 |  
 |  get_property(self, *args, **kwds)
 |      get_property(String)
 |  
 |  gui_about(self, *args, **kwds)
 |      gui_about()
 |  
 |  gui_loadfile(self, *args, **kwds)
 |      gui_loadfile()
 |  
 |  gui_loadsubtitle(self, *args, **kwds)
 |      gui_loadsubtitle()
 |  
 |  gui_play(self, *args, **kwds)
 |      gui_play()
 |  
 |  gui_playlist(self, *args, **kwds)
 |      gui_playlist()
 |  
 |  gui_preferences(self, *args, **kwds)
 |      gui_preferences()
 |  
 |  gui_skinbrowser(self, *args, **kwds)
 |      gui_skinbrowser()
 |  
 |  gui_stop(self, *args, **kwds)
 |      gui_stop()
 |  
 |  help(self, *args, **kwds)
 |      help()
 |  
 |  hide(self, *args, **kwds)
 |      hide([Integer])
 |  
 |  key_down_event(self, *args, **kwds)
 |      key_down_event(Integer)
 |  
 |  loadfile(self, *args, **kwds)
 |      loadfile(String, [Integer])
 |  
 |  loadlist(self, *args, **kwds)
 |      loadlist(String, [Integer])
 |  
 |  menu(self, *args, **kwds)
 |      menu(String)
 |  
 |  osd(self, *args, **kwds)
 |      osd([Integer])
 |  
 |  osd_show_property_te(self, *args, **kwds)
 |      osd_show_property_te(String, [Integer], [Integer])
 |  
 |  osd_show_text(self, *args, **kwds)
 |      osd_show_text(String, [Integer], [Integer])
 |  
 |  pause(self, *args, **kwds)
 |      pause()
 |  
 |  pt_step(self, *args, **kwds)
 |      pt_step(Integer, [Integer])
 |  
 |  pt_up_step(self, *args, **kwds)
 |      pt_up_step(Integer, [Integer])
 |
 |  quit(self, *args, **kwds)
 |      quit([Integer])
 |  
 |  radio_set_channel(self, *args, **kwds)
 |      radio_set_channel(String)
 |  
 |  radio_set_freq(self, *args, **kwds)
 |      radio_set_freq(Float)
 |  
 |  radio_step_channel(self, *args, **kwds)
 |      radio_step_channel(Integer)
 |  
 |  radio_step_freq(self, *args, **kwds)
 |      radio_step_freq(Float)
 |  
 |  run(self, *args, **kwds)
 |      run(String)
 |  
 |  run_command(self, cmd, *args)
 |      Runs a mplayer command.
 |  
 |  screenshot(self, *args, **kwds)
 |      screenshot([Integer])
 |  
 |  seek(self, *args, **kwds)
 |      seek(Float, [Integer])
 |  
 |  seek_chapter(self, *args, **kwds)
 |      seek_chapter(Integer, [Integer])
 |  
 |  set_menu(self, *args, **kwds)
 |      set_menu(String, [String])
 |  
 |  set_mouse_pos(self, *args, **kwds)
 |      set_mouse_pos(Integer, Integer)
 |  
 |  set_property(self, *args, **kwds)
 |      set_property(String, String)
 |  
 |  speed_incr(self, *args, **kwds)
 |      speed_incr(Float)
 |  
 |  speed_mult(self, *args, **kwds)
 |      speed_mult(Float)
 |  
 |  speed_set(self, *args, **kwds)
 |      speed_set(Float)
 |  
 |  step_property(self, *args, **kwds)
 |      step_property(String, [Float], [Integer])
 |  
 |  sub_load(self, *args, **kwds)
 |      sub_load(String)
 |  
 |  sub_log(self, *args, **kwds)
 |      sub_log()
 |  
 |  sub_remove(self, *args, **kwds)
 |      sub_remove([Integer])
 |  
 |  sub_select(self, *args, **kwds)
 |      sub_select([Integer])
 |  
 |  sub_step(self, *args, **kwds)
 |      sub_step(Integer, [Integer])
 |  
 |  switch_ratio(self, *args, **kwds)
 |      switch_ratio([Float])
 |  
 |  switch_vsync(self, *args, **kwds)
 |      switch_vsync([Integer])
 |  
 |  teletext_add_dec(self, *args, **kwds)
 |      teletext_add_dec(String)
 |  
 |  teletext_go_link(self, *args, **kwds)
 |      teletext_go_link(Integer)
 |  
 |  tv_last_channel(self, *args, **kwds)
 |      tv_last_channel()
 |  
 |  tv_set_brightness(self, *args, **kwds)
 |      tv_set_brightness(Integer, [Integer])
 |  
 |  tv_set_channel(self, *args, **kwds)
 |      tv_set_channel(String)
 |  
 |  tv_set_contrast(self, *args, **kwds)
 |      tv_set_contrast(Integer, [Integer])
 |  
 |  tv_set_freq(self, *args, **kwds)
 |      tv_set_freq(Float)
 |  
 |  tv_set_hue(self, *args, **kwds)
 |      tv_set_hue(Integer, [Integer])
 |  
 |  tv_set_norm(self, *args, **kwds)
 |      tv_set_norm(String)
 |  
 |  tv_set_saturation(self, *args, **kwds)
 |      tv_set_saturation(Integer, [Integer])
 |  
 |  tv_start_scan(self, *args, **kwds)
 |      tv_start_scan()
 |  
 |  tv_step_chanlist(self, *args, **kwds)
 |      tv_step_chanlist()
 |  
 |  tv_step_channel(self, *args, **kwds)
 |      tv_step_channel(Integer)
 |  
 |  tv_step_freq(self, *args, **kwds)
 |      tv_step_freq(Float)
 |  
 |  tv_step_norm(self, *args, **kwds)
 |      tv_step_norm()
 |  
 |  use_master(self, *args, **kwds)
 |      use_master()
 |  
 |  vo_border(self, *args, **kwds)
 |      vo_border([Integer])
 |  
 |  vo_ontop(self, *args, **kwds)
 |      vo_ontop([Integer])
 |  
 |  vo_rootwin(self, *args, **kwds)
 |      vo_rootwin([Integer])
 |  
 |  vobsub_lang(self, *args, **kwds)
 |      vobsub_lang([Integer])
 |  
 |  ----------------------------------------------------------------------
 |  Data descriptors defined here:
 | 
 |  angle
 |      angle <int>
 |      [min: 0.0]
 |      select angle
 |  
 |  aspect
 |      aspect <float>
 |      (readonly)
 |  
 |  audio_bitrate
 |      audio_bitrate <int>
 |      (readonly)
 |  
 |  audio_codec
 |      audio_codec <string>
 |      (readonly)
 |  
 |  audio_delay
 |      audio_delay <float>
 |      [min: -100.0] [max: 100.0]
 |  
 |  audio_format
 |      audio_format <int>
 |      (readonly)
 |  
 |  audio_samples
 |      get_audio_samples command
 |      (readonly)
 |  
 |  balance
 |      balance <float>
 |      [min: -1.0] [max: 1.0]
 |      change audio balance
 |  
 |  border
 |      border <flag>
 |      [min: 0.0] [max: 1.0]
 |  
 |  brightness
 |      brightness <int>
 |      [min: -100.0] [max: 100.0]
 |  
 |  channels
 |      channels <int>
 |      (readonly)
 |  
 |  chapter
 |      chapter <int>
 |      [min: 0.0]
 |      select chapter
 |  
 |  contrast
 |      contrast <int>
 |      [min: -100.0] [max: 100.0]
 |  
 |  deinterlace
 |      deinterlace <flag>
 |      [min: 0.0] [max: 1.0]
 |  
 |  demuxer
 |      demuxer <string>
 |      (readonly)
 |      demuxer used
 |  
 |  file_name
 |      get_file_name command
 |      (readonly)
 |  
 |  filename
 |      filename <string>
 |      (readonly)
 |      file playing wo path
 |  
 |  fps
 |      fps <float>
 |      (readonly)
 |  
 |  framedropping
 |      framedropping <int>
 |      [min: 0.0] [max: 2.0]
 |      1 = soft, 2 = hard
 |  
 |  fullscreen
 |      fullscreen <flag>
 |      [min: 0.0] [max: 1.0]
 |  
 |  gamma
 |      gamma <int>
 |      [min: -100.0] [max: 100.0]
 |  
 |  height
 |      height <int>
 |      (readonly)
 |      "display" height
 |  
 |  hue
 |      hue <int>
 |      [min: -100.0] [max: 100.0]
 |  
 |  length
 |      length <time>
 |      (readonly)
 |      length of file in seconds
 |  
 |  loop
 |      loop <int>
 |      [min: -1.0]
 |      as -loop
 |  
 |  meta_album
 |      get_meta_album command
 |      (readonly)
 |  
 |  meta_artist
 |      get_meta_artist command
 |      (readonly)
 |  
 |  meta_comment
 |      get_meta_comment command
 |      (readonly)
 |  
 |  meta_genre
 |      get_meta_genre command
 |      (readonly)
 |  
 |  meta_title
 |      get_meta_title command
 |      (readonly)
 |  
 |  meta_track
 |      get_meta_track command
 |      (readonly)
 |  
 |  meta_year
 |      get_meta_year command
 |      (readonly)
 |  
 |  metadata
 |      metadata <str list>
 |      (readonly)
 |      list of metadata key/value
 |  
 |  mute
 |      mute <flag>
 |      [min: 0.0] [max: 1.0]
 |  
 |  ontop
 |      ontop <flag>
 |      [min: 0.0] [max: 1.0]
 |  
 |  osdlevel
 |      osdlevel <int>
 |      [min: 0.0] [max: 3.0]
 |      as -osdlevel
 |  
 |  panscan
 |      panscan <float>
 |      [min: 0.0] [max: 1.0]
 |  
 |  path
 |      path <string>
 |      (readonly)
 |      file playing
 |  
 |  percent_pos
 |      percent_pos <int>
 |      [min: 0.0] [max: 100.0]
 |      position in percent
 |  
 |  rootwin
 |      rootwin <flag>
 |      [min: 0.0] [max: 1.0]
 |  
 |  samplerate
 |      samplerate <int>
 |      (readonly)
 |  
 |  saturation
 |      saturation <int>
 |      [min: -100.0] [max: 100.0]
 |  
 |  speed
 |      speed <float>
 |      [min: 0.01] [max: 100.0]
 |      as -speed
 |  
 |  stream_end
 |      stream_end <pos>
 |      (readonly) [min: 0.0]
 |      end pos in stream
 |  
 |  stream_length
 |      stream_length <pos>
 |      (readonly) [min: 0.0]
 |      (end - start)
 |  
 |  stream_pos
 |      stream_pos <pos>
 |      [min: 0.0]
 |      position in stream
 |  
 |  stream_start
 |      stream_start <pos>
 |      (readonly) [min: 0.0]
 |      start pos in stream
 |  
 |  sub
 |      sub <int>
 |      [min: -1.0]
 |      select subtitle stream
 |  
 |  sub_alignment
 |      sub_alignment <int>
 |      [min: 0.0] [max: 2.0]
 |      subtitle alignment
 |  
 |  sub_delay
 |      sub_delay <float>
 |  
 |  sub_demux
 |      sub_demux <int>
 |      [min: -1.0]
 |      select subs from demux
 |  
 |  sub_file
 |      sub_file <int>
 |      [min: -1.0]
 |      select file subtitles
 |  
 |  sub_forced_only
 |      sub_forced_only <flag>
 |      [min: 0.0] [max: 1.0]
 |  
 |  sub_pos
 |      sub_pos <int>
 |      [min: 0.0] [max: 100.0]
 |      subtitle position
 |  
 |  sub_scale
 |      sub_scale <float>
 |      [min: 0.0] [max: 100.0]
 |      subtitles font size
 |  
 |  sub_source
 |      sub_source <int>
 |      [min: -1.0] [max: 2.0]
 |      select subtitle source
 |  
 |  sub_visibility
 |      sub_visibility <flag>
 |      [min: 0.0] [max: 1.0]
 |      show/hide subtitles
 |  
 |  sub_vob
 |      sub_vob <int>
 |      [min: -1.0]
 |      select vobsubs
 |  
 |  switch_angle
 |      switch_angle <int>
 |      [min: -2.0] [max: 255.0]
 |      select DVD angle
 |  
 |  switch_audio
 |      switch_audio <int>
 |      [min: -2.0] [max: 255.0]
 |      select audio stream
 |  
 |  switch_program
 |      switch_program <int>
 |      [min: -1.0] [max: 65535.0]
 |      (see TAB default keybind)
 |  
 |  switch_title
 |      switch_title <int>
 |      [min: -2.0] [max: 255.0]
 |      select DVD title
 |  
 |  switch_video
 |      switch_video <int>
 |      [min: -2.0] [max: 255.0]
 |      select video stream
 |  
 |  teletext_format
 |      teletext_format <int>
 |      [min: 0.0] [max: 3.0]
 |      0 - opaque,
 |      1 - transparent,
 |      2 - opaque inverted,
 |      3 - transp. inv.
 |  
 |  teletext_half_page
 |      teletext_half_page <int>
 |      [min: 0.0] [max: 2.0]
 |
 |  switch_angle
 |      switch_angle <int>
 |      [min: -2.0] [max: 255.0]
 |      select DVD angle
 |  
 |  switch_audio
 |      switch_audio <int>
 |      [min: -2.0] [max: 255.0]
 |      select audio stream
 |  
 |  switch_program
 |      switch_program <int>
 |      [min: -1.0] [max: 65535.0]
 |      (see TAB default keybind)
 |  
 |  switch_title
 |      switch_title <int>
 |      [min: -2.0] [max: 255.0]
 |      select DVD title
 |  
 |  switch_video
 |      switch_video <int>
 |      [min: -2.0] [max: 255.0]
 |      select video stream
 |  
 |  teletext_format
 |      teletext_format <int>
 |      [min: 0.0] [max: 3.0]
 |      0 - opaque,
 |      1 - transparent,
 |      2 - opaque inverted,
 |      3 - transp. inv.
 |  
 |  teletext_half_page
 |      teletext_half_page <int>
 |      [min: 0.0] [max: 2.0]
 |      0 - off, 1 - top half,
 |      2- bottom half
 |  
 |  teletext_mode
 |      teletext_mode <flag>
 |      [min: 0.0] [max: 1.0]
 |      0 - off, 1 - on
 |  
 |  teletext_page
 |      teletext_page <int>
 |      [min: 0.0] [max: 799.0]
 |  
 |  teletext_subpage
 |      teletext_subpage <int>
 |      [min: 0.0] [max: 64.0]
 |  
 |  time_length
 |      get_time_length command
 |      (readonly)
 |  
 |  time_pos
 |      time_pos <time>
 |      [min: 0.0]
 |      position in seconds
 |  
 |  tv_brightness
 |      tv_brightness <int>
 |      [min: -100.0] [max: 100.0]
 |  
 |  tv_contrast
 |      tv_contrast <int>
 |      [min: -100.0] [max: 100.0]
 |  
 |  tv_hue
 |      tv_hue <int>
 |      [min: -100.0] [max: 100.0]
 |  
 |  tv_saturation
 |      tv_saturation <int>
 |      [min: -100.0] [max: 100.0]
 |  
 |  video_bitrate
 |      video_bitrate <int>
 |      (readonly)
 |  
 |  video_codec
 |      video_codec <string>
 |      (readonly)
 |  
 |  video_format
 |      video_format <int>
 |      (readonly)
 |  
 |  video_resolution
 |      get_video_resolution command
 |      (readonly)
 |  
 |  vo_fullscreen
 |      get_vo_fullscreen command
 |      (readonly)
 |  
 |  volume
 |      volume <float>
 |      [min: 0.0] [max: 100.0]
 |      change volume
 |  
 |  vsync
 |      vsync <flag>
 |      [min: 0.0] [max: 1.0]
 |  
 |  width
 |      width <int>
 |      (readonly)
 |      "display" width
```