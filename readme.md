# [python] Implementing 24-hour unattended live streaming using Python and FFmpeg

Step 1: It can be your own computer, preferably an idle cloud server.

2. Install Python 3, the specific process is not elaborated on; there are many search solutions available. Note: If it's an installation version for a cloud server, it might be Python 2, and it seems unlikely to support directly uninstalling and installing Python 3.

3. Visit the FFmpeg official website to select the corresponding system for download and compilation installation. Different systems may encounter various issues here. This is a detailed installation process, but everyone's situation is different, so you should use the search engine to solve it. Compiling and installing many things is quite challenging, but once this step is completed, everything will be smooth sailing.

4. After installing FFmpeg, verify by checking the following to confirm success.

-
-
-
-
-
-
-
-
-
-
-

```
$ ffmpeg -versionffmpeg version N-102343-g4d3474432f Copyright (c) 2000-2021 the FFmpeg developersbuilt with gcc 4.8.5 (GCC) 20150623 (Red Hat 4.8.5-44)configuration: --prefix=/root/ffmpeg_build --pkg-config-flags=--static --extra-cflags=-I/root/ffmpeg_build/include --extra-ldflags=-L/root/ffmpeg_build/lib --extra-libs=-lpthread --extra-libs=-lm --bindir=/root/bin --enable-gpl --enable-libfdk_aac --enable-libfreetype --enable-libmp3lame --enable-libopus --enable-libvpx --enable-libx264 --enable-libx265 --enable-nonfreelibavutil      57.  0.100 / 57.  0.100libavcodec     59.  0.100 / 59.  0.100libavformat    59.  0.100 / 59.  0.100libavdevice    59.  0.100 / 59.  0.100libavfilter     8.  0.101 /  8.  0.101libswscale      6.  0.100 /  6.  0.100libswresample   4.  0.
```

5. After ffmpeg is successfully installed and compiled, take my server as an example:
cd home
create an arbitrary directory inside it to store the video
for example, create a directory named "videoList" under "home"
the following is on my server:
[root@iZ0jlcmvdsbq3c2pzlpt2oZ home]# cd huya
[root@iZ0jlcmvdsbq3c2pzlpt2oZ huya]# ls
huya_live.py  nohup.out  videoList
[root@iZ0jlcmvdsbq3c2pzlpt2oZ huya]# pwd
/home/huya
6. The live streaming push script, live.py

-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-

```
import os
```

7. Store the live.py file in the directory level with the video directory that was just created. Of course, this is not a requirement for performance;

8. How to start live streaming: python3 live.py This can be used to start the test window, then the live streaming will be disconnected when the test window is closed.

9. When the test is completed: nohup python3 live_stream.py & At this point, you can close the command window and start the unattended live broadcast.

10. Complete Description: https://blog.csdn.net/u014449096/article/details/140034518?spm=1001.2014.3001.5501

11. Demo address, it is not guaranteed to be available at all times due to my potential suspension or switching of the live streaming address: https://www.huya.com/15732718


## Payment

Here is a pay link on Stripe ( https://buy.stripe.com/3cs8yP7sY87d0vu9AB ). Please contact me lonlonago@foxmail.com after funding $89, and I will send you a complete data files , thank you!

![111.png](111.png)
