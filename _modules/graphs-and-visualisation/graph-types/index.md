---
layout: slideshow
title: Practical Visualization Techniques
slides:

    - content: | 
        ## Practical Visualization Techniques

    - class: left-aligned
      content: |

        ## What types of data?
        {:.center-aligned}

        ### Categorical
        - Nominal
        - Ordinal
        - Interval

        ### Quantitative
        - Ratio (Discrete and continuous)
        


      notes: |
        Common but not only categorisation

        Categorical tells us what and quantitative how much

        Categorical data identifies what we are measuring with numbers. We can often break categorical data into smaller and smaller categories.

        Nominal: labelled data. Apples, oranges, grapes etc. No inherent order. Start applying preferences becomes ordinal. "In name only"

        Ordinal data: Categories with rank. Has intrinsic order. Position in a list or que.
        Some preference. Rank best to worst films or movies of some type

        Interval: Degree of difference between different points. but no ratio between the two. Good example is temperature. Can compare two temperatures, but meaningless to talk about the ratio of one temperature to another

        Ratio: Dealing with full spectrum of comparisons we can make with numbers. Measurements are defined relative to basic unit, and we can have a measurement of zero. Things like speed and time. Ratio of speed, ratio of time taken.

        Why do we care?

        Nature of data informs how we choose to display it.

    - content: |
        ## Displaying Nominal Data

    - content: |
        ## Displaying Ordinal Data

    - content: |
        ## Display

    - content: |
        ## What messages are we sending?
        * Nominal comparison
        * Time Series
        * Ranking and Part-to-Whole
        * Deviation
        * Frequency distribution
        * Correlation
        * Multivariate analysis
        From Stephen Few
      notes: |
        Its helpful to have a framework to think about

    - content: |
        ## Nominal comparison

    - content: |
        ## Time Series
        ![Time series graph](/images/time_series.png)

      notes: |
        Trend. Where are the values going over time. Increasing, Decreasing, Stable?
         Variability. How much do our data values change from observation to observation.
         Rate of change.
         If there is a trend in our data how strong is it. How much change do we expect between each observation or data value.
          Co-variation. 
          How are two time series related to one another. When one series changes how does the other reflect that change. Is it simultaneous or does it lag behind. Does it move in the same direction or the opposite.  
          Cycles. Is there a particularly pattern that repeats over a certain time frame. Does the values always peak at a certain time say 5 minutes after the start of an experiment. 
          Exceptions. When does a data value fall outside the range of what would expect,accounting for trends, cycles and variations. 


    - content: |
        ## Ranking and Part-to-Whole

    - content: |
        ## Deviation

    - content: |
        ## Part-to-Whole

    - content: |
        ## Frequency distribution

    - content: |
        ## Correlation

      notes: |
        Correlation analysis looks at how quantitative variables relate to and affect one another. How do one set of variables vary with regard to another, how much do they vary, how do they vary and why do they vary.

        Want a graphical representation of direction shape and strength of correlation between variables. 

        Scatter plots and scatter plot matrices. 

    - content: |
        ## Multivariate Analysis
        
        ![Parallel co-ordinate plot](/images/parallel_co_ordinate_plot.png)
        {:.fragment}


      notes: |
        WHat happens when we have higher dimensional data? How can we represent the relationship between several different variables in a single graph?

        A number of methods out there but only one is particularly effective - Parallel co-ordinate plots

        Each variable is represented by one of the vertical axis.
        A single, multivalued data value is represented by a line going from point to point on each axis
        Variables are typically normalized so that their min and max     values correspond to the top and bottom of their respective axis


---