---
layout: post
title: Automated Robotic Linkage Mechanism
description:  Worked in a team to design, build, and control a complex linkage mechanism to rapidly press arcade buttons in sequence
skills: 
- signal processing
- transmission design
main-image: /IMG_6858.jpg
---

---
# Project Constraints
Given a preset playing field, our team was responsible for designing the most optimal button pressing linkage to maximize our points within the time limit. Points were scored if the correct button was pressed--the signal for which was provided by an Arduino connected to the playing field. There is a bonus green button that awards more points. It is the only button that is not required to be pressed by the provided 2" by 1/2" by 1/4" acrylic block.

# Motion Generation
## Four-Bar Linkage Mechanism
After multiple trial sketches, our team found a four-bar linkage mechanism which reduced our maximum transmission angle deviation to a mere 7 degrees in two of the three positions. We employed an oblique button pressing mechanism which also reduced the transmission angle deviation further than one which presses the centers.

## Button-Pressing Mechanism
In our design, the provided acrylic block attached to the solenoid via a 3D-printed part that fits to the plunger endpoint geometry.  This then connected to the surface of the acrylic using epoxy. The rails connect to the acrylic piece using an adhesive and go through the coupler. The rails prevent the acrylic piece from being able to rotate on the end of the solenoid plunger. We optimized for moment of inertia to ensure a fast, dynamic response.

<style>
  .pdf-container {
    position: relative;
    width: 100%;
    padding-bottom: 150%; /* Adjust for aspect ratio */
    height: 0;
  }
  .pdf-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: none;
  }

  /* Hide iframe on small screens and show a download link */
  @media (max-width: 768px) {
    .pdf-container { display: none; }
    .mobile-pdf-link { display: block; text-align: center; }
  }
</style>

<div class="pdf-container">
  <iframe src="/assets/images/Full Assembly.pdf"></iframe>
</div>

<p class="mobile-pdf-link" style="display: none;">
  <a href="/assets/images/Full Assembly.pdf" target="_blank">📄 Open PDF</a>
</p>


# Energy Conversion/Transmission
In creating our initial assembly, we chose to minimize the size of our base plate and opted for a compact design thereby reducing the weight of our mechanism. Up to this point, however, we had yet to consider how we were going to move our linkage. We then embarked upon our transmission selection through inertia matching as well as by checking the resolution at the button pressing mechanism, which needs a fine enough sensor resolution to position the button-pressing mechanism where it is intended. The former method yielded a transmission ratio of 1.59 whereas the latter was calculated to be 1.24. Hence, we chose the more conservative 5:3 transmission ratio (1.67:1) for our motor. Thus, we could minimize travel time while meeting speed and torque requirements. Then, onto machining we went!

{% include image-gallery.html images="trancalc.png" height="800" %}

# Safety and Motor Control
A combination of sensors and controllers were used to move our mechanism into the desired positiion/orientation to press each button. This was achieved with an Arduino microcontroller board. For safety, a toggle switch was used in case the mechanism ran into any issues. After assembling our linkage on the playing field and finalizing wiring, we further optimized our performance through PID tuning and adaptive gains.

# Final Performance Video
{% include youtube-video.html id="zZu0kbBJCd0" autoplay = "true" width = "900px" %}
