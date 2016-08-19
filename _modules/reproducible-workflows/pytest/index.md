---
layout: slideshow
title: Introduction to Testing


slides:


  - content: |

      ## Testing frameworks
   
    notes: |
      At this point, you may be wondering that wouldn't it be very time consuming and annoying to run each test function we have written one by one? 

      Software developers being the lazy people they are have use software that automate the testing process. There are several popular testing packages for Python.

  - content: |
      ## Pytest

      - Will sniff out tests that start with "test_" or end with "_test"
      - Easy to use, very powerful

      Pytest is very powerful and has a wide number of features, but is easy to get started with. As you become more proficent with Python, you will find more and more of its features useful. Pytest lets us write tests similar to how we have been doing so in this notebook, writing functions that use assert to compare the output of the tested function against the expected return value. Pytest also test discovery. It will sniff out python test files, any files that start with "test\_" or finish with "\_test" (excluding the .py file extention) will be found and run by Pytest by default.









---