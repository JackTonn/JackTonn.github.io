---
layout: post
title:  Perimeter IC
date:   2025-12-15 17:00:00 -0500
categories: Project
---

<div style="text-align:center;">
  <img
    src="{{ '/assets/images/perimeter_layout.png' | relative_url }}"
    alt="Perimeter Layout"
    width="600">
</div>

## Summary

Visual field testing is an important aspect of ophthalmology as it allows for the evaluation of both central and peripheral vision. It is also used for the detection of some conditions such as glaucoma, retinal damage, or neuropathy. One of the instruments that can be used for this testing is called a perimeter, which involves the presentation of the stimulus in random locations while checking the correct number the patient sees a light. This proposal focuses on the development of a 64-pixel perimeter. This system turns on individual LEDs representing each pixel randomly one at a time, replicating what seems to be random stimuli for the human eyes. To make it more difficult for patients to fix targets, the time is randomly varied between 7 to 20 seconds, ensuring that patient responses are not driven by guesses but by real detection of what they actually see. When the button is pushed within five seconds of the onset of the LED, it is recorded as a “successful detection.” When it is pushed without the presence of a stimulus, it is recorded as “false click” Both of these are counted for the test session. When the test is finished, the total number of positive detection click rates and the total number of false click rates are displayed on a 4-digit seven-segment display. A toggle switch operated by the technician allows the total number of positive or false click rates to be viewed for quicker patient analysis. Finally, another button allows a new test to be initiated while keeping previous test data until the next session. 

For this project, I wrote the Verilog and testbenches for this IC, and acted as the system designer at the top level. I had a groupmate create the analog components, such as a decoder, and clock. This project taught me a lot about writing synthesizeable verilog, and how to design an IC in a team, which was invaluable experience for my senior design project, although this was done in Cadence tools, whereas senior design was done with open source tools.