---
layout: page
title: code
permalink: /code/
---

---

# Neuronal stimulus-response function estimation

## lnpy
A Python package containing many methods for estimating neuronal stimulus-response functions

**Source code:** [https://github.com/arnefmeyer/lnpy](https://github.com/arnefmeyer/lnpy){:target="_blank"}

&nbsp;

---

# Misc

## matcall
A Python package for calling Matlab from Python (using temporary files)

**Source code:** [https://github.com/arnefmeyer/matcall](https://github.com/arnefmeyer/matcall){:target="_blank"}

&nbsp;

## clusterjobs
A Python package that makes running of embarassingly-parallel jobs on high-performance computing clusters quite easy. Currently, the SLURM system is supported (the Sun grid engine (SGE) backend might also work but haven't tested it for a while).

**Source code:** [https://github.com/arnefmeyer/clusterjobs](https://github.com/arnefmeyer/clusterjobs){:target="_blank"}

&nbsp;

---

# Open-ephys plugins

## Frame grabber

![image not found](../images/framegrabber_screenshot.png)

**Description:** A simple video4linux2-based video frame grabber plugin. It retrieves frames from any device supported by [v4l2](http://linuxtv.org/downloads/v4l-dvb-apis/) and displays them using [opencv](http://opencv.org/). Moreover, frames can be saved to disk (in jpg format) together with open-ephys hardware time stamps making it easy to synchronize frames and recorded data later on. Depending on your camera this approach should be useful for most (behavioral) tracking experiments. In case the experiment requires very precise time stamps, e.g., high-speed whisker tracking, it might be a good idea to use a camera that can send TTL pulses for each frame.

**Source code:** [http://www.github.com/arnefmeyer/FrameGrabberPlugin](http://www.github.com/arnefmeyer/FrameGrabberPlugin){:target="_blank"}

&nbsp;

## Virtual Reference

![image not found](../images/virtualref_screenshot_small.png)

**Description:** Implements a virtual reference matrix that is a bit more flexible than open-ephys' channel mapper.

**Source code:** [https://github.com/arnefmeyer/VirtualReferencePlugin](https://github.com/arnefmeyer/VirtualReferencePlugin){:target="_blank"}

&nbsp;

## RPi Camera

![image not found](../images/rpicamera_screenshot.png)

**Description:** A plugin for the [open-ephys plugin-GUI](https://github.com/open-ephys/plugin-GUI/){:target="_blank"} to control a [Raspberry Pi (RPi)](https://www.raspberrypi.org/){:target="_blank"} camera over the network. The camera is controlled locally on the RPi and communication between the recording system and the RPi is done via [zeromq](http://zeromq.org/){:target="_blank"}.

**Source code:** [https://github.com/arnefmeyer/RPiCameraPlugin](https://github.com/arnefmeyer/RPiCameraPlugin){:target="_blank"}

&nbsp;

## Inertia measurement unit (IMU) reader

![image not found](../images/imureader_screenshot.png)

**Description:** APlugin for open-ephys [plugin-GUI](https://github.com/open-ephys/plugin-GUI/){:target="_blank"} to control and read data from an interia measurement unit (IMU) via an Arduino, Teensy, or another compatible microcontroller. Communication between the microncontroller and the IMU sensor is done via i2c.

**Source code:** [https://github.com/arnefmeyer/IMUReaderPlugin](https://github.com/arnefmeyer/IMUReaderPlugin){:target="_blank"}


