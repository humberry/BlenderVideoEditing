# BlenderVideoEditing

Blender 3.4 video proxy settings:

Preview > N > View settings > Proxy Render Size = 50%
and
checked Use Proxies
=> for all video strips/files you will get a proxy file in the selected size of 50%
=> new added video strips/files will only get a proxy in this size => should be set at the beginning

Sequencer > N > Proxy > checked Strip Proxy & Timecode
=> you see all proxy resolutions for this video stripe/file
=> Quality is only for pictures

Be aware that even if you use the "Set selected strip proxies" for chaning resolution and overwrite, the old resolutions won't be deleted, even if they are deselected.

If no directory is chosen you will find the proxies in the "BL_proxy" directory where your .blend file is stored.

When the proxy files are deleted and you run blender again, they won't be created automatically.

So what is the big difference between the view settings and the proxy settings?
The proxy settings are only creating new proxies, but they won't be used if they are not chosen in the view settings.
To keep a long story short:
1) File > New > Video editing
2) Preview > N > View Settings > Proxy Render Size = 25% or 50% > N
3) Happy video editing :)


my video format settings:<br>
File Format = FFmpeg Video<br>
Container = MPEG-4<br>
Video = H.264 (high quality), 1920x1080, 50fps or 60fps, Good (faster) or Slow (smaller file)<br>
Audio = AAC, 44.1kHz or 48kHz, 192bit or MP3, 44.1kHz or 48kHz, 256bit<br>

no H.265 support so far...

[Blender Manual](https://docs.blender.org/manual/en/latest/video_editing/introduction.html)
