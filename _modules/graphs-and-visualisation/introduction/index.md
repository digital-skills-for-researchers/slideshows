---
title: Introduction to Visualization
layout: slideshow
slides:



    - content: |

        # Introduction to Graphs and Visualization 

    - content: |
        ## How are Graphics stored
        Vector and raster graphics

    - content: |
        ## Raster graphics
        ![Look at the pixels!](images/milford_zoom.png)
        notes: |
          alpha channel
          compression

    - content: | 
        ## Bit depth
        ![Look at the pixels!](images/bit_depth.png)

    - content: |
        ## File formats
        + Compressed and uncompressed formats i.e JPEG and PNG
        + Image fidelity vital -> don't compress
        + Intermediate workflow -> don't compress 
        ![Change in levels of JPEG compression](https://upload.wikimedia.org/wikipedia/commons/e/e9/Felis_silvestris_silvestris_small_gradual_decrease_of_quality.png)  
      notes: |
        JPEG is good with smooth changes in colour, rapid changes, such as lines on a graph, can lead to ugly artefacts.   
        IF you are compressing image files, wait until the end of your workflow to do so. Compress once. Repeated compression will degrade your image quality.


    - content: |
        ## Vector graphics
        + Polygons rather than pixels
        + Can scale up as small or large as we want -> rasterize
        ![The difference between a raster and vector graphics](https://upload.wikimedia.org/wikipedia/commons/a/aa/VectorBitmapExample.svg)

    - content: |
        ## Some sort of computational exercise where they play around with colour and bit depth

    - content: |
        ## Colour 


    - class: center-aligned
      background-image: https://upload.wikimedia.org/wikipedia/commons/a/af/RGB_color_solid_cube.png
      background-size: 30%
      background-position: 80%
      content: |
        ## Modelling Colour

        * RGB Colour Model
        * Represents colour as a triple (R,G,B)
        * What most displays use 
        * Device independent implementation
        {:.left-aligned}


    - class: center-aligned
      background-image: https://upload.wikimedia.org/wikipedia/commons/0/0d/HSV_color_solid_cylinder_alpha_lowgamma.png
      background-size: 30%
      background-position: 70%
      content: |
        ## Modelling Colour

        * HSV/HSL Colour Model
        * Designed to be more intuitive than RGB
        * Can convert perfectly back and forth to RGB
        * Represents colour as a triple (H,S,V)

        
    - class: center-aligned
      background-image: https://upload.wikimedia.org/wikipedia/commons/f/f9/CMYK_channels_skala.jpg
      background-size: 30%
      background-position: 70%
      content: |
        ## Modelling Colour

        * Other colour models exist that cover wider range of colour
        * CMYK - 4 channels - used in print





    - content: |

        ## What is Visualization? 


        + It is based on (non-visual) data
        + It produces an image
        + The result is readable and recognizable [Kosara (2007)](http://kosara.net/papers/2007/Kosara_IV_2007.pdf)
            
      notes: |
        Hard to define exactly visualization is. You'll know it when you see it 




    - content: |

        ## Why should we study it?

        * Provide context and link data
        * Develop new insights
        * 

      notes: |
        Effective science communication makes you a better scientist

       
    - class: center-aligned
      background-image: https://upload.wikimedia.org/wikipedia/commons/e/ec/Anscombe%27s_quartet_3.svg
      background-size: 30%
      background-position: 70%
      content: |
        ## New Insights
        Each data set has the same mean and standard deviation




    - content: |

        ## Visualization is an investment

        Effective visualization not only makes your work more understandable to others but to yourself as well.

        Time spent in developing skills in effective visualization will pay itself back many times 

      notes: |
        Over time you will develop a library of techniques that you can use, as well a more literal library of snippets of code that can be re used

    - content: |

        ## Principles of Visualization (From Tufte)

        * Show the data "truthfully", don't distort it
        * Allow the view to understand the most ideas in the shortest time
        * Encourage the viewer to thinking about the form or substance of the data, not the method of display
        * Reveal the structure in the data at a variety of scales
        * Serve a clear purpose within the text or wherever it is displayed
        * Be integrated with other descriptions of the data


    - content: |
        ## The Science of Perception and Visualization

        Human perception important aspect of visualization
        Preattentive processing: low level visual system rapidly processes certain basic features of an image (<200 ms).

        Variety of theories for how and why.

    

    - content: |

        ## The Science of Perception and Visualization

        Pre attentive Processing
        ![alt text](https://www.csc.ncsu.edu/faculty/healey/PP/figs/colour_P.gif)   ![alt text](https://www.csc.ncsu.edu/faculty/healey/PP/figs/colour_A.gif)

      notes: |
        How we process visual information has a big impact on designing effective visualizations



    - content: |

        ## The Science of Perception and Visualization

        Pre attentive Processing
        ![alt text](https://www.csc.ncsu.edu/faculty/healey/PP/figs/conjoin_A.gif)   ![alt text](https://www.csc.ncsu.edu/faculty/healey/PP/figs/conjoin_P.gif)
        


    - content: |

        ## The Science of Perception and Visualization

        ### Further Features
        + Orientation 
        + Size
        + Density 
        {:.left-aligned}


    - content: |
        ![alt text](http://global.qlik.com/~/media/Images/Blog/entries/posts-large/VisualEncoding-Large_625x349.ashx)

    - content: |
        ## Accuracy of visual markers 
        From [Ceveland and McGill](http://www.cs.ubc.ca/~tmm/courses/cpsc533c-04-spr/readings/cleveland.pdf)

        1. Position along a common scale
        2. Positions along non-aligned scales
        3. Length, direction, angle
        4. Area
        5. Volume, curvature
        6. Shading, colour saturation
        {:.left-aligned}
        
      notes: |
        Opinions vary on the exact order

    - content: |
        ## Avoid Chart Junk
        ![alt text](http://1.bp.blogspot.com/-QZRaqE5OK1E/Tyl3KDwofOI/AAAAAAAAAWY/0yyupJsyER8/s1600/F1001E_A_large.gif)
      notes: |
        This is a bit of an oversimplification. Its okay to make a graphic "junkier" if you feel it needs to be more striking or memorable. It is a trade off.
    - content: |

        ## Avoid distortion


    - content: |

        ## Encoding with size

        Graphic dimension <= Data dimension
        ![Don't do this](images/purchasing_power.png)


    - content: |

        ## Small multiples 
        ![alt text](http://danmaclean.github.io/content/images/2015/07/small_multiples.png)      

    - content: |

        ## Small multiples
        ![alt text](https://en.wikipedia.org/wiki/Small_multiple#/media/File:The_Horse_in_Motion.jpg)

    - content: |
        ## Layering and separating
        ![A simple example of layering](images/stravinsky.png)

    - content: |
        ## Colour rules
    

    - content: |

        ## Iterate

        + You are probably not going to get it right the first time.

        + What makes sense to you wont necessarily make sense to others. 

      notes: |
        Creating your figures using script in R/Python etc makes iteration very easy.



    - content: |

        ## Tables

        + If you can effectively convey information with a graph, use a graph

        + Tables still have a place, most often as a reference


    - content: |

        ## General rules for using tables
        * Several smaller tables are better than one large table
        * Structure the table for how your audience will use the data
        * Arrange rows and columns by some sort of context - size, name etc

    - content: | 
        ## Use an Anchor figure
        Hilight the principle data points you want compared to the rest of the data
        ![alt text](http://stats.blogoverflow.com/files/2012/02/table_Feinberg.png)

    - content: | 
        ## Colour lines
        Improves readability remarkably, especially for larger tables
        ![alt text](http://media.24ways.org/2007/07/illi_7.gif)


    - content: | 
        ## Combine Tables and Graphs
        Show trends/patterns in data as well as exact values
        ![alt text](http://www.perceptualedge.com/images/example2improvedsolution.GIF)


    - content: |
        ## Sparklines   
        Show shape and variation of data 
        ![alt text](http://i.stack.imgur.com/C463D.png)

    - content: |
        ## Visualizing high dimensional/ complex data    

        ![alt text](https://c1.staticflickr.com/7/6142/5920564485_d34dbc2549_b.jpg)


    - content: |
        ## Visualizing high dimensional/ complex data  
        ![alt text](https://archinate.files.wordpress.com/2015/05/edu-workshop-tableaupublic-datadriven1.png)

    - content: |
        ## Explore your options, there is a whole [zoo](http://queue.acm.org/detail.cfm?id=1805128) of choices out there
        There might not be an established solution yet  ¯\\_(ツ)_/¯ so be creative

--- 