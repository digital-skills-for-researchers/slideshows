---
layout: slideshow
title: Introduction to Programming with Python
slides:

    - content: |
        ## Perception of colour
        ![Colour Sensitivty](https://upload.wikimedia.org/wikipedia/commons/9/94/1416_Color_Sensitivity.jpg)

      notes: |
        Three types of colour receptor. Tuned to Short medium and long wave
        When light comes falls on the retina, the different receptors will respond at different levels depending on their tuning. Combining their output creates the perception of the colour of the light. 

        From the sensitivity graph you have probably noticed that we have an even response across the spectrum of visible colour. If you sum up the response curves you'll see that we perceive greenish colours more brightly.

    - content: |
        # Colour
      notes: |
        An extremely important technical aspect of visualization is how do we represent colour? What is a computational representation of colour that we can store and manipulate? 

        To represent colour digitally we use a _colour model_. A colour model aims to represent a wide range of colours using a few primary colours that are mixed in some way.




    - class: center-aligned
      background-image: https://upload.wikimedia.org/wikipedia/commons/a/af/RGB_color_solid_cube.png
      background-size: 30%
      background-position: 80%
      content: |
        ## Modelling Colour

        * RGB  Colour Model
        * Represents colour as a triple (R,G,B)
        * What most displays use 
        * Device independent implementation
        {:.left-aligned}
      notes: |

        The colour model you are most likely to be familiar with is the RGB model. In the RBG model we represent colour a a triple of three numbers, with one number for each of Red, Green and Blue.

        It's handy to know how the RBG model works as this is the most common colour model used in displays. Nearly all displays have three colours per pixel or point on the screen, which produce red, green or blue light.

        Something important to note about RGB is that the actual implementation, how each colour gets reproduced on a screen, is up to the maker of the screen. No two types of screens will reproduce the same RGB value in the same way. A certain shade of green on one screen will be slightly different on another. This is pretty noticeable when creating a series of slides on a laptop and then going and playing them through a projector.

        We visualize the colour space of RGB as a cube. Each corner of the cube has each colour at full strength or zero strength, with colours inside the cube having values in between. Visualizing the RBG cube highlights that it is fairly unintuitive way to think about colour. Trying to adjust colours in  RGB for a desired affect is not a straightforward process.

        . 


    - class: center-aligned
      background-image: https://upload.wikimedia.org/wikipedia/commons/0/0d/HSV_color_solid_cylinder_alpha_lowgamma.png
      background-size: 30%
      background-position: 50% 90%
      content: |
        ## Modelling Colour

        * HSV (Hue Saturation Value)/HSL (Hue Saturation Lightness) Colour Models
        * Designed to be more intuitive than RGB
        * Can convert perfectly back and forth to RGB
        * Represents colour as a triple (H,S,V)


      notes: |
        The HSL and HSV are alternative representations of the RGB colour model. They were designed to be a more intuitive way of viewing the RGB colour spectrum. 

        In the HSL model the Hue of the colour is a angle between 0 and 360 degrees.  The Luminance is the brightness of the colour, 0% Luminance is black and 100% Luminance is white, with darker and lighter shades of the colour between.

        HSV 

        
    - class: center-aligned
      background-image: https://upload.wikimedia.org/wikipedia/commons/f/f9/CMYK_channels_skala.jpg
      background-size: 30%
      background-position: 70%
      content: |
        ## Modelling Colour

        * Other colour models exist that cover wider range of colour
        * CMYK (Cyan, Magenta, Yellow, Key) - 4 channels 
        * Pantone
    
      notes: |
        To make things more confusing, print uses different model(s) to digital. Most printed images use CMYK to produce images. CMYK is a _subtractive_ rather than _additive_ process, unlike RGB. The base colour is black (key) and colours are filtered out to create the spectrum of colour. 

        Finally, some things are printed in pantone colours, which use a specific set of colours with defined pigments. THe benefit of pantone colours is that the colour will be similar from printer to printer as they all have the same standard to follow.



---