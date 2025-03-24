## Example HLS for playback from mp4 file

Generate HLS from MP4 file

```sh
ffmpeg -i ../SampleVideo_1280x720_30mb.mp4 -map 0 -c copy -f hls -hls_time 5 -hls_list_size 0 -hls_segment_filename output%03d.mp4 output.m3u8        ─╯
ffmpeg version 7.1 Copyright (c) 2000-2024 the FFmpeg developers
  built with Apple clang version 16.0.0 (clang-1600.0.26.4)
  configuration: --prefix=/opt/homebrew/Cellar/ffmpeg/7.1_4 --enable-shared --enable-pthreads --enable-version3 --cc=clang --host-cflags= --host-ldflags='-Wl,-ld_classic' --enable-ffplay --enable-gnutls --enable-gpl --enable-libaom --enable-libaribb24 --enable-libbluray --enable-libdav1d --enable-libharfbuzz --enable-libjxl --enable-libmp3lame --enable-libopus --enable-librav1e --enable-librist --enable-librubberband --enable-libsnappy --enable-libsrt --enable-libssh --enable-libsvtav1 --enable-libtesseract --enable-libtheora --enable-libvidstab --enable-libvmaf --enable-libvorbis --enable-libvpx --enable-libwebp --enable-libx264 --enable-libx265 --enable-libxml2 --enable-libxvid --enable-lzma --enable-libfontconfig --enable-libfreetype --enable-frei0r --enable-libass --enable-libopencore-amrnb --enable-libopencore-amrwb --enable-libopenjpeg --enable-libspeex --enable-libsoxr --enable-libzmq --enable-libzimg --disable-libjack --disable-indev=jack --enable-videotoolbox --enable-audiotoolbox --enable-neon
  libavutil      59. 39.100 / 59. 39.100
  libavcodec     61. 19.100 / 61. 19.100
  libavformat    61.  7.100 / 61.  7.100
  libavdevice    61.  3.100 / 61.  3.100
  libavfilter    10.  4.100 / 10.  4.100
  libswscale      8.  3.100 /  8.  3.100
  libswresample   5.  3.100 /  5.  3.100
  libpostproc    58.  3.100 / 58.  3.100
Input #0, mov,mp4,m4a,3gp,3g2,mj2, from '../SampleVideo_1280x720_30mb.mp4':
  Metadata:
    major_brand     : isom
    minor_version   : 512
    compatible_brands: isomiso2avc1mp41
    creation_time   : 1970-01-01T00:00:00.000000Z
    encoder         : Lavf53.24.2
  Duration: 00:02:50.86, start: 0.000000, bitrate: 1474 kb/s
  Stream #0:0[0x1](und): Video: h264 (Main) (avc1 / 0x31637661), yuv420p(progressive), 1280x720 [SAR 1:1 DAR 16:9], 1086 kb/s, 25 fps, 25 tbr, 12800 tbn (default)
      Metadata:
        creation_time   : 1970-01-01T00:00:00.000000Z
        handler_name    : VideoHandler
        vendor_id       : [0][0][0][0]
  Stream #0:1[0x2](und): Audio: aac (LC) (mp4a / 0x6134706D), 48000 Hz, 5.1, fltp, 383 kb/s (default)
      Metadata:
        creation_time   : 1970-01-01T00:00:00.000000Z
        handler_name    : SoundHandler
        vendor_id       : [0][0][0][0]
Stream mapping:
  Stream #0:0 -> #0:0 (copy)
  Stream #0:1 -> #0:1 (copy)
Output #0, hls, to 'output.m3u8':
  Metadata:
    major_brand     : isom
    minor_version   : 512
    compatible_brands: isomiso2avc1mp41
    encoder         : Lavf61.7.100
  Stream #0:0(und): Video: h264 (Main) (avc1 / 0x31637661), yuv420p(progressive), 1280x720 [SAR 1:1 DAR 16:9], q=2-31, 1086 kb/s, 25 fps, 25 tbr, 90k tbn (default)
      Metadata:
        creation_time   : 1970-01-01T00:00:00.000000Z
        handler_name    : VideoHandler
        vendor_id       : [0][0][0][0]
  Stream #0:1(und): Audio: aac (LC) (mp4a / 0x6134706D), 48000 Hz, 5.1, fltp, 383 kb/s (default)
      Metadata:
        creation_time   : 1970-01-01T00:00:00.000000Z
        handler_name    : SoundHandler
        vendor_id       : [0][0][0][0]
Press [q] to stop, [?] for help
[hls @ 0x12970dcb0] Opening 'output000.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output001.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output002.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output003.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output004.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output005.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output006.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output007.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output008.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output009.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output010.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output011.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output012.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output013.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output014.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output015.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output016.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output017.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output018.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output019.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output020.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output021.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output022.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output023.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output024.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output025.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output026.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output027.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output028.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output029.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output030.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output031.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output032.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[hls @ 0x12970dcb0] Opening 'output033.mp4' for writing
[hls @ 0x12970dcb0] Opening 'output.m3u8.tmp' for writing
[out#0/hls @ 0x600003cc8000] video:22650KiB audio:8008KiB subtitle:0KiB other streams:0KiB global headers:0KiB muxing overhead: unknown
frame= 4271 fps=0.0 q=-1.0 Lsize=N/A time=00:02:50.84 bitrate=N/A speed=4.57e+03x
```
