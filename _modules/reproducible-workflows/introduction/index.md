---
layout: slideshow
title: Introduction to Testing


slides:


  - content: |

      # Testing
   
    notes: |
      Focus on testing today


      Testing is a crucial part of software development.

      Whether we are part way writing some software or have potentially completed our software - how do we ensure that what we have done is correct.

      Testing is a deep topic, can take a while to pick up.

      Best way to learning is by discussing why why are doing this and then hands on practice

      During this less going to be less of me talking and more of you doing.

      You are not going to get it right the first time every time, going to learn by making mistakes

      Not going learn everything in one lecture, going to learn and consolidate over the remainder of the semester. 

      Please stop me at any point to ask questions.

  - content: |

      ## Checklists

    notes: |
      So this mentality, of checking to make sure whatever process or product we are doing or creating is everywhere. Think of a checklists. 
      We have checklists in all areas of life. Take driving for example. You want to overtake someone. Space, Speed, other cars, road surface.
      An industry that's famous for checklists is aviation. Aviation has a pretty remarkable safety record, you are much safer in a 747 than driving. A famous part of the aviations safety focussed culture are checklists. In aviation having not checked something can be a matter of life or death.


  
  - content: |
      ## Create a Take Off checklist

      ![Cessna](images/cessna.jpg){: height="500"}

    notes: |
      Lets go through an example. You own a light place like the one shown. YOu are about to fly somewhere, say Auckland to Wellington. What do you check before you do?   What's on your take-off check-list?

      Get into groups of two or three and write down a few points with your group. Spend a few minutes doing this.

      Who can share something with me something they wrote

      Have printed list



  - content: |
      # Do we test in science?
    notes: |
      Lets move to some more familiar territory. A lot of you will have conducted experiments of some sort. 

      When you are conducting an experiment, do you know that is has worked?
      I'm not a scientist, so you tell me. How do you know
      [Discussion]

      A lot of researchers,as Fabiana can attest, verify the results of their experiments when they get a result that they expect to see. This goes for software as well 

      time in design, controls and calibration  >> time spent doing the experiment

      The same goes for software, you should spend much more time thinking about design, what problems you are trying to solve, and testing your software than the time you spend writing it up

  - content: |
      # How could we test software  

    notes: |
      So you all have had some experience writing small pieces of software now. So we have been talking about how testing for a bit now. So how would you test software. What would you want to test.How could you test it. Not knowing is okay. Act is though  you were an exam and this question came up and you were doing your best to get some marks.

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
      Unit tests, which what we will be focussing on today. Unit tests are about testing individual units of code, functions basically, and verifying the output is what we expect.

      Regressing is going backwards, so a regression test tests that our software is going backwards. As we develop our software things are going to change. We want to make sure that our software continues to behave as it use to and still works. Regression testing is for checking that as we tried to fix one thing we dint break another. 

      Integration testing is where we test that the different components of our software work together as a group. Integration tests check that the major part of the systems work together correctly.

      There are a lot more tests out there as well. 

      Enough time talking about tests. Lets start talking about how to write them.







---