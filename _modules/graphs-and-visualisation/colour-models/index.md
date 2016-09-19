---
layout: slideshow
title: Colour
slides:


    - content: |
        ### Perception of colour
        ![Colour Sensitivty](https://upload.wikimedia.org/wikipedia/commons/9/94/1416_Color_Sensitivity.jpg){: .center-aligned height="400"}

      notes: |

        In retina three types of cells exist that are used to perceive light, rods, cones and some other cells that dont have a short name. Cones are the cells responsible for the peception of colour. 

        Three types of colour receptor cells. Tuned to Short medium and long wave lengths.

        When light comes falls on the retina, the different receptors will respond at different levels depending on their tuning. 

        Combining their output creates the perception of the colour of the light. 

        From the sensitivity graph you have probably noticed that we have an even response across the spectrum of visible colour. If you sum up the response curves you'll see that we perceive greenish colours more brightly.

    - content: |
        # Colour
      notes: |
        An extremely important technical aspect of visualization is how do we represent colour? What is a computational representation of colour that we can store and manipulate? 

        To represent colour digitally we use a _colour model_. A colour model aims to represent a wide range of colours using a few primary colours that are mixed in some way.

    - content: |
        ### Modelling Colour

        * RGB  Colour Model
        * Represents colour as a triple (R,G,B)
        * What most displays use 
        * Device independent implementation

        ![RGB Cube](https://upload.wikimedia.org/wikipedia/commons/a/af/RGB_color_solid_cube.png){: .center-aligned height="400"} 

      notes: |

        The colour model you are most likely to be familiar with is the RGB model. In the RBG model we represent colour a a triple of three numbers, with one number for each of Red, Green and Blue.

        It's handy to know how the RBG model works as this is the most common colour model used in displays. Nearly all displays have three colours per pixel or point on the screen, which produce red, green or blue light.

        Something important to note about RGB is that the actual implementation, how each colour gets reproduced on a screen, is up to the maker of the screen. No two types of screens will reproduce the same RGB value in the same way. A certain shade of green on one screen will be slightly different on another. This is pretty noticeable when creating a series of slides on a laptop and then going and playing them through a projector.

        We can visualize the colour space of RGB as a cube. Each corner of the cube has each colour at full strength or zero strength, with colours inside the cube having values in between. Visualizing the RBG cube highlights that it is fairly unintuitive way to think about colour. Trying to adjust colours in  RGB for a desired affect is not a straightforward process.

        

    - content: |
        ### Modelling Colour
        * HSV (Hue Saturation Value)/HSL (Hue Saturation Lightness) Colour Models
        * Designed to be more intuitive than RGB
        * Can convert perfectly back and forth to RGB
        * Represents colour as a triple (H,S,V)
        ![HSV](https://upload.wikimedia.org/wikipedia/commons/0/0d/HSV_color_solid_cylinder_alpha_lowgamma.png){: .center-aligned height="400"} 


      notes: |
        The HSL and HSV are alternative representations of the RGB colour model. They were designed to be a more intuitive way of viewing the RGB colour spectrum. RGB is useful when we are describing how to produce colours in a computer monitor, but now how to make a shade of green slightly more blue tinged for example. It is highly unintuitive for design purposes. 

        In the HSL model the Hue of the colour is a angle between 0 and 360 degrees. Hue represents moving along the visible range of colour, from red  to yellow, green, blue, purple and then back to red  The Luminance is the brightness of the colour, 0% Luminance is black and 100% Luminance is white, with darker and lighter shades of the colour between.

        In HSV  we have Hue which works in the same way as HSL. Saturation is the distance from the neutral colour on the grey black-axis to a pure hue, and value is where the colour sites of the grey-black axis.

        There are advantages and disadvantages to both models relative to one another. Colour picking in software seems to arbitrarily pick one or the other, or sometimes both. 

        While HSL/HSV let us describe colour in perceptual manner, they are not perceptually uniform. (Example?)



    - content: |
        ### Modelling Colour

        * Other colour models exist that cover wider range of colour
        * CMYK (Cyan, Magenta, Yellow, Key) - 4 channels 
        * Pantone
        ![CMYK](https://upload.wikimedia.org/wikipedia/commons/f/f9/CMYK_channels_skala.jpg){: .center-aligned height="400"}
                         

      notes: |
        To make things more confusing, print uses different model(s) to digital. Most printed images use CMYK to produce images. CMYK is a _subtractive_ rather than _additive_ process, unlike RGB. The base colour is black (key) and colours are filtered out to create the spectrum of colour. 

        Finally, some things are printed in pantone colours, which use a specific set of colours with defined pigments. THe benefit of pantone colours is that the colour will be similar from printer to printer as they all have the same standard to follow.

    - content: |
        ### Practical Rules for Colour

        Use color only when needed to serve a particular communication goal.

    - content: |
        ### Colour rules

      notes: |

        Use color only when needed to serve a particular communication goal.
        We should only add color to an information display to achieve something in particular
        Colour should be used meaningfully
        Use different colors only when they correspond to differences of meaning
        in the data.
        When adding colour to a graph, think what is the purpose of this colour

    - content: |
        ## Showing Detail

      notes: |
        The key rule  for the use of colour in data visulizsation, luminance contrast is needed. Pairing black and white leads to the biggest contrast in brightness. The smaller the graphic we are dealing with, the greater the contrast we need. Likewise if our graphic is large it's not quite anything goes but you have a lot more leeway. 

        We also use luminance contrast as a way to manage the viewers attention.

        The aspects of our visualization with the highest contrast is where our attention will be drawn first.  Likewise features with lower contrast will be comparatively less noticeable.

        It helps to think of luminance contrast as as finite resource. We only have so much we can spend on our graphic, so we should think wisely about what features we want to invest in.

        A general rule is there should be a ratio a luminance ratio of 3:1 between text or graphics to the background 

        WC3 0.299 * R + 0.587 * G + 0.114 * B


    - content: |
        ### Avoid Oversaturation
        ![Argh](http://www.infragistics.com/community/cfs-filesystemfile.ashx/__key/CommunityServer.Blogs.Components.WeblogFiles/tim_5F00_brock.Maria_5F00_Blogs.Spring_5F00_2016/7762.bar1.png){width="200"} 

        ![Better](http://www.infragistics.com/community/cfs-filesystemfile.ashx/__key/CommunityServer.Blogs.Components.WeblogFiles/tim_5F00_brock.Maria_5F00_Blogs.Spring_5F00_2016/2465.bar2.png){width="400"}
      
      notes: |



        When we look at a graphic with too much saturated colour, it can be almost painful. 

        Using muted colours is alot easier on our eyes, particularly for anything thats going to displayed on a screen.

        Being selective with saturated colours lets us emphasis and hi light aspects of our data more easily. Our eyes focus on differences in saturation, rather than absolute values.  Allowing for a greater range in saturation will let things pop out more. 

        When dealing with smaller aspects of a graph, such as markers on a time series, we can be more liberal with the use of saturated colour without making our graph too garish. Likewise with small symbols we can should boost the luminance contrast. 

    - content: |
        ### Colour Coding Information

      
      notes: |
        A key function of the use of colour in data viz is to encode information. First use is to enforce distinctness between categories of data, so that we can distinguish between different categories. The second is learnability, that the viewer comes to understand that one colour indicates a particular category of data. 

        There are strong limits on how many distinct colours can be used on a graphic so a viewer can reliably understand what each colour is encoding. A number of different numbers have been reported between 6 and 12. The more colours we have the less easily we can distringuish between them, it gets easier to confuse one colour for another.

        If we are using soley grey scale colours we need to limit ourselves to four colours. 



    - content: |
        ### Colour maps/palettes

      notes: |

        How we we choose a effective colour palette for our graphs

        The typical/default colour map or palette used in Scientific Visualization is the rainbow colour map (Red, Orange, Yellow, Green, Blue, Indigo, Violet)

        The big issue with the Rainbow colour map is that it is not perceptually ordered. To remember the ordering most people use a mnemonic Roy G Biv or the like. In studies where people have been asked to place them in order the orderings they come up with vary. If asked to sort a series of shades of grey they place them in order of lightness to darkest, or the reverse. If your data has some sort of ordering, the rainbow colour map wont convent that. 

        Perhaps one advantage of the rainbow colour map is familiarity, people are accustomed to seeing and interpreting it. And it is pretty and quite striking.

        When choosing a colour map here are some principles we should follow

        – The map yields images that are aesthetically pleasing.
        – The map has a maximal perceptual resolution.
        – The order of the colours should be intuitively the same for all people.
        – The perceptual interpolation matches the underlying scalars of the map.
        - distinct for all people, including colour-blind readers;
        - distinct from black and white;
        - distinct on screen and paper;

        From [Kenneth Moreland  ](https://cfwebprod.sandia.gov/cfdocs/CompResearch/docs/ColorMapsExpanded.pdf)

        Here are some tools which can help you pick or create a colour map

        http://colorbrewer2.org/
        https://color.adobe.com/create/color-wheel/
        http://tools.medialab.sciences-po.fr/iwanthue/  
        http://www.mrao.cam.ac.uk/~dag/CUBEHELIX/cubetry.html
        http://paletton.com/

        Matplotlib has changed default colour map, see here for a [talk](https://www.youtube.com/watch?v=xAoljeRJ3lU) on why 

    - content: |
        ### The Rainbow Colourmap
        ![Don't use this](http://i.stack.imgur.com/uAyax.png){: .center-aligned height="400"}   

    - content: |
        ### Perceptually Uniform colourmaps
        ![Isn't this better!](http://pong.tamu.edu/~kthyng/movies/txla_plots/salt/2010-07-30T00.png){: .center-aligned height="400"}   

    - content: |
        ### Background Colour - Grey or White?
        ![Hadley Wickham](http://i.stack.imgur.com/4pNJl.png){: .center-aligned height="400"}

    - content: | 
        ### Background Colour - Grey or White?
        ![Nate Silver](http://i.stack.imgur.com/CrO7k.png){: .center-aligned height="400"}    

      notes: |
        May seem like a trite question

        Hadley Wickham

        "The grey background gives the plot a similar colour (in a typographical sense) to the remainder of the text, ensuring that the graphics fit in with the flow of a text without jumping out with a bright white background. Finally, the grey background creates a continuous field of colour which ensures that the plot is perceived as a single visual entity."

        Reduced screen glare

        Alot Colour maps been designed with a white background (for printing) in mind. Their perceptual properties will differ against a darker background.

        Also using a white background allows you to optimise a graph for both electronic display and printing, rather than having to prepare a different printer-friendly version.


---