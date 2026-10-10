---
layout: post
title:  Highly Configurable Mechanical Accelerometer
date:   2026-06-30 17:00:00 -0500
categories: Project
---

<div style="text-align:center;">
  <img
    src="{{ '/assets/images/accelerometer_payload.jpg' | relative_url }}"
    alt="Accelerometer Payload"
    width="600">
</div>

## Summary

As a part of the payload subteam of Cyclone Rocketry, we get to design a scientific experiment to fly in the rocket. The experiment must fit in a standard size of 10cm x 10cm x Ycm, with Y being a multiple of 10 between 10 and 60. We designed ours to be a 3U, so 10 x 10 x 30 cm.

Functionally, the accelerometer works by hanging a mass between springs. Then, that mass is connected to a potentiometer, whose output is routed to an analog to digital converter (ADC), which is then stored on an SD card for post processing. The decision to do post processing instead of live inflight processing was made because it allowed for us to be using the microcontroller minimally, thus increasing out battery life with low power modes. I was in charge of the software and hardware design for the payload, along with ideating the mechanical design. This project taught me more about working with noisy sensors, as our created sensor was quite noisy, and writing small, dependable software that can run for hours on end in variable environments.

Unfortunately, this payload was not quite functional, as during acceleration, the batteries would depress into the spring below them, causing power to be lost. Thus, the data from the launch was lost. More can be read in our post-flight data report, seen below.
<iframe
    src="{{ '/assets/documents/Team703DataAnalysis-1.pdf' | relative_url }}"
    width="100%"
    height="800">
</iframe>

A massive thank you goes out to the team that helped me see my idea become a reality. Without their mechanical design knowledge, this would not have been possible! 

Team Lead: [Gigi Karner](https://www.linkedin.com/in/georgia-karner-334121179)

Team Members: [Jacob Gray](https://www.linkedin.com/in/jacob-gray-00b040292), [Carly Scolaro](https://www.linkedin.com/in/carly-scolaro-1a1223383), [Ethan DeBrower]()