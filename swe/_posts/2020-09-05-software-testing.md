---
title: "Software Testing: What is it, Why do we need it and what are the different types?" 
permalink: /swe/:title
collection: swe
category: swe
date: 16 December 2023
---

Software testing is an important step during its development lifecycle. It ensures that the software function or operate as what the stakeholders wanted, which contribute to the perception of quality software. Failure to properly test a software can lead to disastrous consequences, especially if the software is running in an environment where lives are stake or is responsible for the financial health of an organisation or nation.

### What is testing?

Software testing is the process in which a piece of software, be it a module, component or an application, is verified and validated. In other words, it is the process to make sure a piece of software is:

1. Built right *(Verified)*
2. The right thing that the user will want to use *(Validated)*

There are two ways to go about software testing; one is automated testing and the other manual testing.

Automated testing is done to automate certain repetitive but necessary tasks in a formalised testing process, or to perform additional tests that would be difficult to do manually.

On the other hand, manual testing is done by testers playing the roles of the users to identify defects in the software that the automated testing missed. A written test plan is followed by the tester to ensure completeness of a test.

In the latter part of this article, we will look at the different types of testing and how they are done.

### Why testing is important

Now, you know what is testing but you may be wondering why it is important. Let us use a simple scenario to illustrate the importance of testing.

> A highly-reputable medical device manufacturer, AXT, designed and sells a new surgical robot equipped with a laser scalpel mounted on an arm. The scalpel can cut through the human skin and tissues with precision. The control panel for the robot comes with two joysticks. The one on the left moves the robotic arm along the vertical plane (up or down) while the one on the right moves the robotic arm along the horizontal plane (forward, backwards, left and right).
>
> For the left joystick, AXT stated that for every 1 degree tilt forward or backwards shall move the arm down or up by the same amount in centimetres. AXT also stated that every 5 degree tilt of the right joystick in any direction shall move the arm in the respective direction by one-fifth of an inch.
>
> After seeing several live demonstrations done on dummies and receiving good feedbacks from trials that involved some of the surgeons from Tea General Hospital, the hospital finally bought one such surgical robot from AXT for their new operating theatre. Technicians from AXT went to the hospital installed it in the new operating theatre, indicated on the official checklist stating they have verified that the robot was working.
>
> Three days later, a surgeon who's trained to use the surgical robot decided to use it to perform a brain surgery on a young patient. With the patient lying on the operating bed, the surgeon powered on the robot and started manipulating the joysticks. He moved the right joystick to bring the scalpel end of the arm above the patient. It worked as intended. Then, the surgeon moved the left joystick, shifting it forward to lower the arm. Even though the joystick has a tilt of five degrees, the arm plunged downwards and hit the patient in the face with the laser scalpel punching through the skull into the brain.
>
> The patient died on the spot, leaving the parents extremely distraught and the surgeon traumatised. The surgeon quit his job a day later and was found dead on the ground floor of his apartment building two days later, having jumping off from his kitchen window on the ninth floor.
>
> An investigation later revealed that the technicians did not test the robot and checked off the checklist confidently, assuming that they have done it correctly. They believed in their installation and setup skills as they have done it many times for other hospitals. If they have tested the robot in the first place, they would have found that they failed to connect the signal regulator for the module that controlled the robot arm's vertical movement.

The scenario described above maybe seems like it came from some horror movies but it does reflect the reality of what will happen when software system, or any system for that matter, is not tested thoroughly.

### Different types of software testing

Software testing can be divided two different categories: functional and non-functional testing.

Functional testing is a quality assurance process that checks the individual software component does what it is supposed to. For example, if a calculator software says it can determine the sum of two numbers, then a check will be performed to verify that it return the correct sum for any two numbers.

On the other hand, non-functional testing checks the way the software operates. Using the calculator example, a non-functional requirement would specify that the calculator has to return a result within a second. So, if the calculator takes up to 20 seconds to return the correct result, it is technically functional. However, who would use a calculator that takes a longer time than a human to calculate the sum of two numbers?

#### Functional testing

**Unit testing**

Unit testing is a type of functional testing that tests a piece of software using Unit Tests, which are automated tests written and run by software developers to verify that a section of the software meets its design and behaves correctly. Generally, they are written to cover specific core functions within the application and ensure the functions return the correct response from a given set of inputs.

With continuous delivery and continuous testing, unit tests form a big part of that process since they are used to verify that every section of the software they covered behave correctly. In the event that there are failing tests, this would indicate that certain functionalities within the application has not been implemented properly by the developers.

**Smoke testing**

Smoke testing is a type of testing that verifies a software is built correctly and it can run. It is commonly used to reveal any simple failures and allowing a prospective software release to be rejected.

Unlike the other type of testing, smoke testing is supposed to run quickly, to give the benefit of faster feedback. This way, developers can quickly fix what went wrong and get the next build ready.

**Integration testing**

Applications have grown increasingly complex with a lot of moving parts. Integration testing is a type of testing that verifies the different parts are able to come together and work. One way it does that is by ensuring the interfaces between the different software components are defect free and they can communicate with each other correctly.

**Exploratory testing**

In contrast to other type of functional testing, exploratory testing is a type of informal testing that is more ad-hoc and freestyle, relying more on the tester's creativity instead of following scripted test cases. The term exploratory testing was coined by Cem Kaner in 1984.

With exploratory testing, it is all about discovery, investigation and learning while the test is happening. It is up to the tester to come up with new test cases as they navigates through an application. This help to ensure that software bugs that were not picked up by other type of testings are identified and resolved.


#### Non-functional testing

**Usability testing**

Usability testing measures the ease-of-use of an application by testing it on users who have never seen or used it before. If an application has good design intuitiveness, users would less likely to be confused by it, thus are more likely to use it.

To do usability testing, a scenario or a realistic situation need to be setup where the user can perform a series of tasks on the application being tested. Observers will watch and take notes. In addition, other test instruments such as scripted instructions, paper prototypes and questionnaires are also used to gather feedback. Another popular testing method is the Think Aloud Protocol where users will vocalise what they are thinking about as they navigate through the application and how they will be performing an action.

**Performance Testing**

Performance testing determines how well an application performs. A non-functional requirement given by the users could specify that able to execute an action and return a result or give a response to the user within some time limit. In this case,  it would fall under performance test coverage.

Using the calculator example mentioned earlier, a simple performance test can be conducted using a stop watch and a tester using the calculator to calculate the sum of two numbers. The stop watch will start counting once the user press the "=" button. When the calculator screen shows the result, the stop watch is stopped immediately. Then, the time taken could be record as part of a performance test report.

**Stress testing**

A modern application generally perform quite well on modern machines and could handle several dozen of people using it. However, when the number increases to several hundred  or even several thousands users per minute, the application might not even function. It might start crashing due to limited hardware resources.

Stress testing is about putting the application under heavy load and finding out what is the breaking point. With that information, the amount and type of resources to be provisioned can be done more effectively to ensure availability of the application, or that developers can improve the application in terms of its error handling and prevent it from crashing due to insufficient computation resource, thus improving its robustness.

