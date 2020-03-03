---
title: FrameGrabber open-ephys plugin
layout: post
featured: /assets/images/framegrabber_screenshot.png
link: http://www.github.com/arnefmeyer/FrameGrabberPlugin
---


**FrameGrabber** - a simple video4linux2-based video frame grabber plugin. It retrieves frames from any device supported by [v4l2](http://linuxtv.org/downloads/v4l-dvb-apis/) and displays them using [opencv](http://opencv.org/). Moreover, frames can be saved to disk (in jpg format) together with open-ephys hardware time stamps making it easy to synchronize frames and recorded data later on. Depending on your camera this approach should be useful for most (behavioral) tracking experiments. In case the experiment requires very precise time stamps, e.g., high-speed whisker tracking, it might be a good idea to use a camera that can send TTL pulses for each frame.
