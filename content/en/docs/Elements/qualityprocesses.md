---
title: "16. Quality Processes"
description: "What processes are in place that impact the quality of your software?"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 160
---

### Quality Processes
We create software solutions in order to solve business problems, or to make money from our solutions.  Therefore it is important that the solutions we create do what our customers want them to do, are delivered in a timely manner, and function satisfactorily.  Every software development team hopes they are creating solutions with the quality desired by their customers, and most teams develop techniques, practices, and processes to improve the quality of the software they deliver.  It is not far from the truth to claim that the goal of most literature about software, and especially most literature about software development processes, has the primary goal of guiding people to create software of higher quality.  Each of the elements in this document about the software development context should be evaluated by software development teams primarily because good practices for each element can improve the quality of speed with which software is delivered.  Solo developers providing a solution to a single end user may do little other than testing the code themselves, or reviewing it for accuracy.  Large organizations implement many practices to improve software quality.  These practices include all the practices referenced elsewhere in this document when you are considering which practices are best for your context.  Some of those include:  Pair programming, code reviews, automated testing, TDD, quick feedback via CI/CD, and static code analysis.  Other practices include simply having a quality assurance team of people, and training developers to create higher quality output.
The amount of effort organizations invest in improving quality is not simply a reflection of how much they care, but also of other factors in their software development context.  We hope that teams developing applications on which the lives of others depend place a lot of effort into delivering quality solutions, but a team delivering a static web site to list the services provided by a local dentist may invest much less in practices that increase software quality.  Increasing quality usually comes with increasing costs, and companies often decide what level is good enough based on the number of customers affected and how severely they are affected, along with considering other projects and software solutions they could be working on that might provide a better return on investment. 


##### How do you test software?
* Developers manually test
* We have some staff occasionally manually test
* We have someone that specializes in testing
* We can run some automated tests
* We have an extensive set of tests we can run to cover almost everything important
* We auto run tests when changes are committed
* We auto run tests when changes are pushed to a central repo
* We auto run tests on a regular schedule


##### Quality Dimensions
* Functional correctness
* Performance
* Reliability
* Usability
* Security

##### Quality Activities
* Code reviews
* Automated testing
* Exploratory testing
* Performance benchmarking

##### Anti‑Patterns
* Testing only at the end
* No definition of done
* Manual testing only
* Ignoring non‑functional requirements

##### Templates
* Quality strategy
* Test plan
* Definition of done checklist