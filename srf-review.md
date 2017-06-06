---
layout: page
title: SRF review
permalink: /SRF review/
---

---

# Models of neuronal stimulus-response functions: elaboration, estimation and evaluation

Arne F. Meyer, Ross S. Williamson, Jennifer F. Linden, and Maneesh Sahani

Front. Syst. Neurosci. doi: 10.3389/fnsys.2016.00109 

**Link:** [Link to article](http://journal.frontiersin.org/article/10.3389/fnsys.2016.00109/abstract)

## Abstract
Rich, dynamic, and dense sensory stimuli are encoded within the
nervous system by the time-varying activity of many individual neurons.
A fundamental approach to understanding the nature of the encoded
representation is to characterise the function that relates the
moment-by-moment firing of a neuron to the recent history of a complex
sensory input.
This review provides a unifying and critical survey of the techniques
that have been brought to bear on this effort thus far --- ranging
from the classical linear receptive field model to modern approaches
incorporating normalisation and other nonlinearities.
We address separately the structure of the models; the criteria and
algorithms used to identify the model parameters; and the role of
regularising terms or "priors".  In each case we consider benefits
or drawbacks of various proposals, providing examples for when these
methods work and when they may fail. Emphasis is placed on key
concepts rather than mathematical details, so as to make the
discussion accessible to readers from outside the field.
Finally, we review ways in which the agreement between an assumed
model and the neuron's response may be quantified.
Re-implemented and unified code for many of the methods, and example
data sets, are made freely available.

## Code
A Python package containing [many methods](http://www.frontiersin.org/files/Articles/223015/fnsys-10-00109-HTML/image_m/fnsys-10-00109-t001.jpg) 
for estimating neuronal stimulus-response functions is available on github ("srf-review" branch).

**Source code:** [https://github.com/arnefmeyer/lnpy](https://github.com/arnefmeyer/lnpy)

