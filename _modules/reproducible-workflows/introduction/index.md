---
layout: slideshow
title: Introduction to Testing


slides:


  - content: |

      # Testing
   
    notes: |
      Focus on testing today
      Testing is a crucial part of software development
      Whether we are part way writing some software or have potentially completed our software - how do we ensure that what we have done is correct. 
      Last week you saw assert statements, which we can use to check whether things we need to be true for our program to work are in fact so. Have we successfully opened the file, is our data valid etc 


  - content: |

      ## Checklists

    notes: |
      So this mentality, of checking to make sure whatever process or product we are doing or creating is everywhere. Think of a checklist. 
      We have checklists in all areas of life. Take driving for example. You want to overtake someone. Space, Speed, other cars, road surface.
      An industry thats famous for checklists is aviation. Aviation has a pretty remarkable safety record, you are much safer in a 747 than driving. A famous part of the aviations safety focussed culture are checklists


  
  - content: |
      ## Create a Take Off Checklist

      ![Cessna](images/cessna.jpg){: height="500"}

    notes: |
      Lets go through an example. You own a light place like the one shown. YOu are about to fly somewhere, say auckland to new pylmouth. What do you check before you do?   What's on your takeoff checklist?

      Have print off of list



  - content: |
      # Do we test in science?
    notes: |
      Lets take this closer to home. Alot of you will have conducted experiments of some sort. 

      When you are conducting an experiment, do you know that is has worked?
      I'm not a scientist, so you tell me. How do you know
      [Discussion]

      Alot of researchers,as Fabiana can attest, verify the results of their experiments when they get a result that they expect to see. This goes for software as well 

      time in design, controls and calibration  >> time spent doing the experiment

      The same goes for software, you should spend much more time thinking about design, what problems you are trying to solve, and testing your software than the time you spend writing it up

  - content: |
      # How could we test software  

    notes: |
      So you all have had some experience writing small pieces of software now. So we have been talking about how testing for a bit now. So how would you test software. What would you want to test.How could you test it [Discussion]

      How could we test?
      A website
      Opening a file
      A simulation - CFD  

  - content: |
      ## Wide variety of tests used in software
      - Unit tests
      - Regression tests
      - Integration test
      - And (many) more

    notes: |
      Unit tests, which what we will be focussing on today. Unit tests are about testing indivual units of code, functions basicaly, and verifying the output is what we expect.

      Regressing is going backwards, so a regression test tests that our software is going backwards. As we develop our software things are going to change. We want to make sure that our software continues to behave as it use to and still works. Regression testing is for checking that as we tried to fix one thing we didnt break another. 

      Integrartion testing is where we test that the differenet components of our software work togtether as a group. Integrartion tests check that the major part of the systems work together correctly.

      There are alot more tests out there as well. 

      Enough time talking about tests. Lets start talking about how to use them.







---