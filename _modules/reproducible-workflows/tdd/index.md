---
layout: slideshow
title: Test Driven Development


slides:


  - content: |

      # Test Driven Development
   
    notes: |
      So what we have been working to talking about is a process called Test Driven Development. Test Driven Development is a software development process. If we think back to the lectures on project management, the traditional way of developing software is in a waterfall style. Test Driven development is an agile style of software development.

      Almost all software projects are attempting do something that hasn't been done before. That something new could be creating a new technology, applying an existing technology in a new domain, or people or an organisation doing something they haven't done previously.

      Science comparison



      When you are writing software you often won't fully understand the technology you are using upfront, in your case this is probably very true, as you are learning how to program probably for the first time. 

      For the people you are building software for, this process can be even more painful. Taking a process you do perform based on experience and convention and translating it to software means having working towards having an exact specification can be really difficult.

      Building software is a learning process. There are going to misunderstandings along the way. There are going to be changes along the way. We want a development process that can handle these unanticipated changes. 

      To handle these changes we need some sort of a feedback loop. As we develop new features and new versions of our software we want to establish whats working and what isnt. The sooner we can get feedback about this the more quickly we can work to fix and improve our software.
      One way to get feedback quickly is if we have written our tests up front. Test Driven Development inverts the development process. Tests are written first. Tests are written to drive design. We specify the behaviour we want based on our tests, and write code to meet these specifications.


  - content: |

      ## The TDD Cycle
      ![The TDD Cycle](images/tdd_cycle.png){: height="500"}

    notes: |

      So this all sounds nice in theory. But how does it work in practice?

      The cycle of writing software with TDD is often summed up into three steps. Red, Green, Refactor.

      Red: Write a test that doesn't run Think about what you want your code to accomplish and write a test as though the code already exists. Don't write new functionality without having a failing test.
      
      Green: Make the test work quickly Write enough code to make the test past. A common refrain at this stage is 'YAGNI' (You Ain't Gonna Need It'). Don't try and generalize to quickly. Once all your tests are passed you are finished with this stage.

      Refactor: Make it right Clean up your code and remove unnecessary duplication while ensuring that you continue to pass all tests. When we refactor we are improving the quality of our code without changing its external behaviour. From outside the code you pass in the same arguments and receive the same results. The code does what it did before but it is easier to read, understand its purpose and debug

  - content: |
      ## This sounds a bit like science..

    notes: |

      Starting a theory
      One of the most difficult aspects of creating a theory is working out exactly which aspect of the world you want the theory to coherently explain. A theory can begin as a vague hypothesis.

      Likewise in TDD the customer you are building the software for may not really know what the problem they are trying to solve is, and this problem needs to be clarified



      In science you start with a theory. 
      Tests take the role of experiments

      Software design takes to the place of theory

      Reproducibility:

      Experimental Reproducibility is managed through continued use of automated tests

      In TDD small steps are used so it is clear what caused the tests to fail. This is similar to how a control tries to ensure a single change in an experiment.

      Theory simplicity:
      In science we apply Occam's razor, like in TDD we want to choose the simplest thing that could possibly work

      Theory building is a social process.
      For a scientific theory to become accepted it must survive scrutiny. Science doesn't move smoothly like the idealized vision it likes to present itself. Scientists can unconsciously and consciously bias their experiments, misanalyse, misinterpret and avoid results that show their ideas are wrong or faulty.

      In TDD we try to avoid this issues. Tests are written up front, we are trying to avoid wishful thinking about how things go by stating upfront what expect. 



  
  - content: |
      ## Why TDD

      
    notes: |

      TDD keeps us focussed. No speculation. YAGNI.

      Systemic, process. Never doubt about what do do next.

      It is a runnable form of the specification.

      This mean that you can see from the test cases:

      THAT the code being called full-fills the specification as the results expected are right there in the test cases. Visual inspection (which expects the test cases to pass) can say immediately "oh, this test checks that calling invoiceCompany given this situation, should have THAT result".
      
      HOW the code should be called. The actual steps needed to do the tests are specified directly without any external scaffolding (databases are mocked out etc).

      Since you have the specification on runnable form, you are done when the full test suite passes. You may add more tests as you clarify things on a more detailed level, but as a basic principle you have a very clear and visible indicator of progress and when you are done.

      This means that you can tell when work is necessary or not (does it help pass a test) you end up needing to do less.

      TDD is not the only agile software development methodology out there, and it's not necessarily the best. But you will build better software following a rigorous process. 


  - content: |
      ##  TDD is not an excuse to not do design

    notes: | 
      A high level architecture is general still advised, just not with too much detail. Big Up Front Design is discouraged, but doing just enough design is encouraged. Remember back to when we were talking about Agile and Scrum. Incremental development and release. We are using tests to help specify the design at a lower level, we still need to spend time thinking about high level design.

   
 

  - content: |
      # Writing good tests


    notes: |

      Writing good tests isn't magic. There are a number of practices we can follow to help write better tests. Switching to writing our tests up front doesn't suddenly mean we will be writing good tests. 

  - content: |
      ## Writing good tests in TDD
      - Test a single concept
      - It should be automated and repeatable.
      - It should be easy to implement.
      - It should be relevant tomorrow.
      - Anyone should be able to run it at the push of a button.
      - It should run quickly.

  - content: |
      ## More tips on writing good tests   
      - It should be consistent in its results 
      - It should have full control of the unit under test.
      - It should be fully isolated.
      - When it fails, it should be easy to detect what was expected and determine how to pinpoint the problem.

    notes: |
      It should be consistent in its results. It always returns the same result if you don’t change anything between runs

      Some other external system shouldn't influence its behaviour. 

      It should be fully isolated (runs independently of other tests).


  - content: |
      ## Naming tests
    
    notes: |
      So far we have been lumping all our tests together inside a single function. There are a couple of issues with this. When a test fails, the remaining tests in the function  will not be run, as our test function will have encountered an error. Secondly, its hard to know exactly which test failed and why, we have to inspect the arguments we passed to our palindrome function to work out what we we were testing. So the first thing we need to do is split our tests into different functions, one function per test. After that we need to name our functions so that we can work out what they are testing solely based on the name. 

      So how do we name our test functions? There are no hard and fast rules, but a common way to name a test is **test\_\[test\_name\]**, where **test_name** describes in particular what we are testing. Following these conventions our palindrome tests would look like the following




---