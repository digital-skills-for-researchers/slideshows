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
          How are two time series related to one another. When one series changes how does the other reflect that change. Is it simaltaneous or does it lag bhind. Does it move in the same direction or the opposite.  
          Cycles. Is there a particuarl pattern that repeats over a certain time frame. Does the values always peak at a certain time say 5 minutes afer the start of an experiemtn. 
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


---