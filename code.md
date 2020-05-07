---
layout: page
title: Code, tools etc
order: 4
---

This page contains some of the code and tools that I have developed during my
research. Everything is free to use, modify, and distribute (see also [this open source letter](http://opensourceforneuroscience.org/){:target="_blank"}).


- [Neuronal stimulus-response function estimation](#srf)
- [The Mousecam](#mousecam)
- [Open-ephys plugins](#oeplugins)
- [Miscellaneous](#misc)


<hr class="hr-thick-wide" />


### <a name="srf"></a>Neuronal stimulus-response function estimation

<!-- <div style="display: table; width:100%;">
    <div style="display: table-cell; vertical-align: top; height: 50px; width: 25%;">
    <a href="https://github.com/arnefmeyer/lnpy"><img src="/public/example_multifilt_ln_model_simplified.png" alt="github lnpy" />
    </a>
    </div>
    <div style="display: table-cell; vertical-align: middle; height: 50px; width: 75%;">
    <b>lnpy</b> - a Python package containing many methods for estimating neuronal stimulus-response functions. For descriptions of the underlying models and estimators see:
    </div>
</div> -->

![coding model](/public/images/example_multifilt_ln_model_simplified.png)

**lnpy** -- a Python package containing many methods for estimating neuronal stimulus-response functions. For descriptions of the underlying models and estimators see:  

_Models of neuronal stimulus-response functions: elaboration, estimation and evaluation_  
Meyer AF, Williamson R, Linden JF, and Sahani M  
Front. Syst. Neurosci., 2017, 10, 109
([article](http://journal.frontiersin.org/article/10.3389/fnsys.2016.00109/full){:target="_blank"})

_Fast and robust estimation of spectro-temporal receptive fields using stochastic approximations_  
Meyer AF, Diepenbrock JP, Ohl FW, and Anemüller J  
J Neurosci Methods, 2015, 246, 119-133
([article](http://www.sciencedirect.com/science/article/pii/S0165027015000618){:target="_blank"})

_Temporal variability of spectro-temporal receptive fields in the anesthetized auditory cortex_  
Meyer AF, Diepenbrock JP, Ohl FW, and Anemüller J  
Frontiers in Computational Neuroscience, 2014, Vol. 8(165) ([article](http://journal.frontiersin.org/article/10.3389/fncom.2014.00165/abstract){:target="_blank"})

_Discriminative Learning of Receptive Fields from Responses to Non-Gaussian Stimulus Ensembles_  
Meyer AF, Diepenbrock JP, Happel MF, Ohl FW, and Anemüller J  
PLOS ONE, 2014, Vol. 9(4), pp. e93062
([article](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0093062){:target="_blank"})

<a href="https://github.com/arnefmeyer/lnpy" target="_blank" class="button">Source code/files</a>


<hr class="hr-thick-wide" />


### <a name="mousecam"></a>The Mousecam

![mouse with eye cameras and implant](/public/images/mousecam.png)

The mousecam is a head-mounted camera system that integrates detailed behavioral monitoring with electrophysiological (or optical) recordings in freely moving mice.
<!-- It is now part of the awesome [Open Ephys](https://open-ephys.org/){:target="_blank"} project. -->

_A head-mounted camera system integrates detailed behavioral monitoring with multichannel electrophysiology in freely moving mice_  
Meyer AF\*, Poort J\*, O'Keefe J, Sahani M, Linden JF  
Neuron, 2018, 100, 46-60
([article](https://www.cell.com/neuron/fulltext/S0896-6273(18)30822-5){:target="_blank"})

<a href="https://open-ephys.org/mousecam" target="_blank" class="button">Source code/files</a>


<hr class="hr-thick-wide" />


### <a name="oeplugins"></a>Open-ephys plugins

<!-- #### RPiCamera
<div style="display: table; width:100%;">

    <div style="display: table-cell; vertical-align: top; height: 50px; width: 25%;">
    <img src="/public/oeplugins/rpicamera_screenshot.png" alt="github lnpy" width="90%"/>
    </div>

    <div style="display: table-cell; vertical-align: middle; height: 50px; width: 75%;">
    <p>
A plugin for the <a href="https://github.com/open-ephys/plugin-GUI/" target="_blank">
 open-ephys plugin-GUI</a> to control a <a href="https://www.raspberrypi.org" target="_blank">Raspberry Pi (RPi)</a> camera over the network. The camera is controlled locally on the RPi and communication between the recording system and the RPi is done via <a href="http://zeromq.org/" target="_blank"> zeromq</a>.
    </p>
    <p>
      <a href="https://github.com/arnefmeyer/RPiCameraPlugin" target="_blank" class="button">Source code/files</a>
    </p>
    </div>

</div> -->


#### RPiCamera
![](/public/oeplugins/rpicamera_screenshot.png)

A plugin for the [open-ephys plugin-GUI](https://github.com/open-ephys/plugin-GUI/){:target="_blank"} to control a [Raspberry Pi (RPi)](https://www.raspberrypi.org/){:target="_blank"} camera over the network. The camera is controlled locally on the RPi and communication between the recording system and the RPi is done via [zeromq](http://zeromq.org/){:target="_blank"}.

<a href="https://github.com/arnefmeyer/RPiCameraPlugin" target="_blank" class="button">Source code/files</a>


---
#### IMU Reader
![](/public/oeplugins/imureader_screenshot.png)

Plugin for open-ephys [plugin-GUI](https://github.com/open-ephys/plugin-GUI/){:target="_blank"} to control and read data from an interia measurement unit (IMU) via an Arduino, Teensy, or another compatible microcontroller. Communication between the microncontroller and the IMU sensor is done via i2c.

<a href="https://github.com/arnefmeyer/IMUReaderPlugin" target="_blank" class="button">Source code/files</a>


---
#### VirtualRef
![](/public/oeplugins/virtualref_screenshot_small.png)

Implements a virtual reference matrix that is a bit more flexible than open-ephys' channel mapper
(but requires more processing power).

<a href="https://github.com/arnefmeyer/VirtualReferencePlugin" target="_blank" class="button">Source code/files</a>


---
#### EventPublisher
![](/public/oeplugins/eventpublisher_screenshot_space.png)

A plugin for publishing events (TTL, messages) in plain text over the network.

<a href="https://github.com/arnefmeyer/EventPublisherPlugin" target="_blank" class="button">Source code/files</a>


---
#### FrameGrabber
![](/public/oeplugins/framegrabber_screenshot.png)

A simple video4linux2-based video frame grabber plugin. It retrieves frames from any device supported by [v4l2](http://linuxtv.org/downloads/v4l-dvb-apis/) and displays them using [opencv](http://opencv.org/). Moreover, frames can be saved to disk (in jpg format) together with open-ephys hardware time stamps making it easy to synchronize frames and recorded data later on. Depending on your camera this approach should be useful for most (behavioral) tracking experiments. In case the experiment requires very precise time stamps, e.g., high-speed whisker tracking, it might be a good idea to use a camera that can send TTL pulses for each frame.

<a href="http://www.github.com/arnefmeyer/FrameGrabberPlugin" target="_blank" class="button">Source code/files</a>


<hr class="hr-thick-wide" />


### <a name="misc"></a>Miscellaneous

#### clusterjobs

A Python package that makes running of embarassingly-parallel
jobs on high-performance computing clusters quite easy. Currently, the SLURM
system is supported (the Sun grid engine (SGE) backend might also work but
haven't tested it for a while).

<a href="https://github.com/arnefmeyer/clusterjobs" target="_blank" class="button">Source code/files</a>



---
#### matcall

A Python package for calling Matlab from Python (using temporary files).

<a href="https://github.com/arnefmeyer/matcall" target="_blank" class="button">Source code/files</a>
