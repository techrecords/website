---
title: ESP32-based project, streams live I2S-microphone data over WiFi Access Point
featured_image: _images/ap-audio-streamer/webserer-page-small.png
post_date: 2026-05-11 12:00:00
post_excerpt: his project might be a good start if you want a device that streams...
comment_status: closed
taxonomy:
    category: Projects
    post_tag:
        - esp32
        - i2s
        - websocket
        - platformio
        - vibecoding
---

This project might be a good starting point if you want a device that streams audio data to many listeners — for example, audio streaming for excursions, guided tours, etc.

I had a few iterations with this project. The first iteration started in 2024; I was experimenting with Raspberry Pi and gstreamer at that time. I couldn't beat the high latency of web streaming — obviously the issue was that httpd wasn't configured to use websockets. I abandoned this idea afterwards. Back in 2026, after switching to ESP32, I was able (with AI help) to reach a desirable result. It supports 10 simultaneous connections. [HERE](https://github.com/techrecords/ap-audio-streamer) you can find the repo with the project and all HOWTOs in [README.md](https://github.com/techrecords/ap-audio-streamer/blob/main/README.md).

![Picture of ap-audio-streamer hardware](/_images/ap-audio-streamer/hw-view-small.jpg "Picture of ap-audio-streamer hardware") {.wp-post-image}

Links related to the project:

- [ESP32-S3](https://www.espressif.com/en/products/socs/esp32-s3)
- [WebSockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API)
- [PlatformIO](https://platformio.org/)