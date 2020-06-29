# gst-hlssink2 - GStreamer fMP4 HLS Sink
GStreamer HLS fMP4 sink

GStreamer hlssink2 element that uses mp4mux in splitmuxsink rather than mpegtsmux. 

As fMP4s are the futture for HTTP Adaptive Bit Rate Streaming and with the fMP4 support in HLS dating back to 2016, the need for a fMP4 based HLS sink in GST is the need of the hour. With GStreamer having nice elements like splitmuxsink with mp4mux, denying fragmented MP4 output for HLS is a great sin.

This elemets outputs fMP4s instead of the traditional MPEG-2 TS and only supports Live HLS profile. The m3u8's version is also increased to HLS 4.0 to support fMP4.

This code can be built similar to the other gst-good-plugins either using menson or automake.

The output fMP4s have been tested with the following HLS players
* hls.js
* Google shaka-player.js
* Chrome extension Native HLS Playback

Compatible GStreamer version 1.14 and above
