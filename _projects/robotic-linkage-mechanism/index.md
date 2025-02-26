---
layout: post
title: Robotic Linkage Mechanism
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

# Energy Conversion/Transmission
In creating our initial assembly, we chose to minimize the size of our base plate and opted for a compact design thereby reducing the weight of our mechanism. Up to this point, however, we had yet to consider how we were going to move our linkage. We then embarked upon our transmission selection through inertia matching as well as by checking the resolution at the button pressing mechanism, which needs a fine enough sensor resolution to position the button-pressing mechanism where it is intended. The former method yielded a transmission ratio of 1.62 whereas the latter was calculated to be 1.24. Hence, we chose the more conservative 5:3 transmission ratio (1.67:1) for our motor. Thus, we could minimize travel time while meeting speed and torque requirements. Then, onto machining we went!

# Safety and Motor Control
A combination of sensors and controllers were used to move our mechanism into the desired positiion/orientation to press each button. This was achieved with an Arduino microcontroller board. For safety, a toggle switch was used in case the mechanism ran into any issues. After assembling our linkage on the playing field and finalizing wiring, we further optimized our performance through PID tuning and adaptive gains.

# Final Performance Video

## Embedding images 
### External images
{% include image-gallery.html images="https://live.staticflickr.com/65535/52821641477_d397e56bc4_k.jpg, https://live.staticflickr.com/65535/52822650673_f074b20d90_k.jpg" height="400"%}
<span style="font-size: 10px">"Starship Test Flight Mission" from https://www.flickr.com/photos/spacex/52821641477/</span>  
You can put in multiple entries. All images will be at a fixed height in the same row. With smaller window, they will switch to columns.  

### Embeed images
{% include image-gallery.html images="project2.jpg" height="400" %} 
place the images in project folder/images then update the file path.   


## Embedding youtube video
The second video has the autoplay on. copy and paste the 11-digit id found in the url link. <br>
*Example* : https://www.youtube.com/watch?v={**MhVw-MHGv4s**}&ab_channel=engineerguy
{% include youtube-video.html id="MhVw-MHGv4s" autoplay= "false"%}
{% include youtube-video.html id="XGC31lmdS6s" autoplay = "true" %}

you can also set up custom size by specifying the width (the aspect ratio has been set to 16/9). The default size is 560 pixels x 315 pixels.  

The width of the video below. Regardless of initial width, all the videos is responsive and will fit within the smaller screen.
{% include youtube-video.html id="tGCdLEQzde0" autoplay = "false" width= "900px" %}  

<br>

## Adding a hozontal line
---

## Starting a new line
leave two spaces "  " at the end or enter <br>

## Adding bold text
this is how you input **bold text**

## Adding italic text
Italicized text is the *cat's meow*.

## Adding ordered list
1. First item
2. Second item
3. Third item
4. Fourth item

## Adding unordered list
- First item
- Second item
- Third item
- Fourth item

## Adding code block
```ruby
def hello_world
  puts "Hello, World!"
end
```

```python
def start()
  print("time to start!")
```

```javascript
let x = 1;
if (x === 1) {
  let x = 2;
  console.log(x);
}
console.log(x);

```

## Adding external links
[Wikipedia](https://en.wikipedia.org)


## Adding block quote
> A blockquote would look great if you need to highlight something


## Adding table 

| Header 1 | Header 2 |
|----------|----------|
| Row 1, Col 1 | Row 1, Col 2 |
| Row 2, Col 1 | Row 2, Col 2 |

make sure to leave aline betwen the table and the header
