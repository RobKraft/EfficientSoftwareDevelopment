---
title: "Continuous Integration"
description: "Considerations of how your context impacts your ability to gain value from continuous integration"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 50
---

### What is continuous integration?
Although there are minor variations to the meaning of continuous integration, most agree it means launching a build process every time some code is committed or pushed to a central repository; or at least running the build process on a build server many times throughout the day based on the code in a primary repository.  Here is the [Wikipedia](https://en.wikipedia.org/wiki/Continuous_integration) definition.  The automation of devops usually roughly follows this pattern:
1. Automate builds
2. Automate running of tests
3. Continuous Integration
4. Continuous Deployment (to test/QA) 
5. Continuous Deployment to Prod (for contexts with this goal)

Therefore, many of the elements affecting the automation of devops affects the implementation of continuous integration in the same way.

### How does your context affect the success you will have implementing continuous integration?
###### 1. How does the *[Organizational Structure](/docs/elements/orgstructure/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
How your organization is structured has no impact on your team's ability to implement continuous integration.
###### 2. How does the *[Development Team Culture](/docs/elements/devculture/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
Only a dysfunctional culture, very resistant to change with individuals unwilling to share what they know for fear of losing their jobs (once others can do what they do) is likely to oppose implementing continuous integration.
###### 3. How does the *[Hiring Process](/docs/elements/hiringprocess/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
Your organization's hiring process has no impact on your team's ability to implement continuous integration.
###### 4. How does the *[Team Composition](/docs/elements/teamcomposition/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
Your team's composition has no impact on your team's ability to implement continuous integration, other than the potential lack of knowledge about how to get started and make it happen that more experienced developers can provide.
###### 5. How does the *[Training Provided on Code](/docs/elements/trainingoncoding/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The training your organization provides on code languages and tools has a small impact on your team's ability to implement continuous integration.  If your company wants this automation, the company will hopefully allow the developers to be trained to do it with their tools.
###### 6. How does the *[Training Provided on 'Our Ways of Doing Things'](/docs/elements/trainingonourways/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The training your team provides on your way of doing things has no impact on your team's ability to implement continuous integration.
###### *7. How does the *[Environment](/docs/elements/environment/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
See the response below related to DevOps.
###### 8. How does the *[Project Selection](/docs/elements/projectselection/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The way in which projects are selected has no impact on your team's ability to implement continuous integration.
###### *9. How does the *[Solution Purpose](/docs/elements/solutionpurpose/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
One of the few factors that affects the ability to implement continuous integration is the purpose of the solution.  If you are building a temporary solution, something that will be used once and will be completed soon, then CI may not be worth the time.  Prototypes, demo applications, technical proofs of concept, and solutions that produce a single report or output and are then discarded may not benefit from CI.
###### 10. How do the *[Application Architecture Priorities](/docs/elements/apparchpriorities/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
Your application's architecture priorities has no impact on your team's ability to implement continuous integration
###### 11. How do the *[Security Demands](/docs/elements/securitydemands/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The security demands of your solution have no impact on your team's ability to implement continuous integration.
###### 12. How do the *[Requirements, Features, and Priorities](/docs/elements/rqmtsandfeatures/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The way your team manages requirements, features, and priorities has no impact on your team's ability to implement continuous integration
###### 13. How do the *[Regulations](/docs/elements/regulations/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The regulations your organization must comply with has no impact on your team's ability to implement continuous integration.
###### 14. How does *[Who Decides What To Do](/docs/elements/whodecides/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
Who decides what to do next on your teams has no impact on your team's ability to implement continuous integration.
###### 15. How does *[Project Management](/docs/elements/projectmanagement/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
How your team manages projects and tasks has no impact on your team's ability to implement continuous integration.
###### 16. How do the *[Quality Processes](/docs/elements/qualityprocesses/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The processes you use to insure quality in your application have no impact on your team's ability to implement continuous integration.  But continuous integration and the regular running of tests can provide a lot of improvement in quality to your solution through quicker feedback to developers.
###### 17. How does the *[Architecture Forecasting](/docs/elements/architectureforecasting/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The plans you have for evolving the architecture of your application have no impact on your team's ability to implement continuous integration.
###### *18. How do your *[DevOps](/docs/elements/devops/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The automation of builds can be performed on the same computers developers use to code and debug.  But to implement a CI process with frequent builds and test runs usually requires a separate server to handle the workload so that developers computers aren't slowed down when the processes run, and so that they can build using the code everyone in team has committed, not just the code from one developers computer.  Today, a lot of teams spin up build servers in the cloud to do this.  It can also be done with a traditional server on-premise or in the cloud.  Either way, teams need to be skilled enough to set up and configure the build servers and maintain the build environment, which often also means creating test databases for automated testing processes.  Teams with development based in the cloud generally have an advantage over teams doing all their builds and processes on computers on premise.
###### 19. How does the *[Architecture](/docs/elements/architecture/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The architecture of your application has no impact on your team's ability to implement continuous integration
###### *20. How does the *[Code](/docs/elements/code/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
Some types of coding don't have build processes, such as low-code environments or Visual Basic macro script inside of Microsoft Excel.  And some other languages, particularly scripting languages, don't need to be built, but some developers do execute them in test environments against a set of tests after the code is committed to a repo.
Your code repositories can impact your ability to implement CI.  Some older source code control tools are not as flexible as git and lack good tooling to run well in cloud or integrations to manage a build and test pipeline.  Adopting CI may include changing to different tools for source code control and code management.
###### *21. How does the *[Code Quality](/docs/elements/codequality/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The current quality of your application has no impact on your team's ability to implement continuous integration, unless your builds and tests take so long to run that these CI builds and tests can only run once per day or less.  This can happen with extremely large code bases that are all fully built together every time, or when tests make database calls or other actions that cause the tests to run for a long time.  In such cases, teams may consider just doing partial builds, or changing the tests to only run the slow ones weekly, or rewriting the tests and code so the tests can run faster.
###### 22. How does the *[Application Quality](/docs/elements/appquality/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The current quality of your application has no impact on your team's ability to implement continuous integration.
###### 23. How does the *[Deployment Environment](/docs/elements/deployenvironment/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
The environment into which your software is deployed may have some impact on your ability to implement CI, primarily because the environments don't support builds.  Some examples include scripting languages, low-code environment, and Excel macros.  Other examples are software written that talks directly to physical devices such as phones, GPS devices, and Arduino controllers.  However, many of the most popular languages and hardware devices that you can write software for also have emulators/simulators that allow you to deploy code to a simulated environment for testing, and you may be able to add some automation there, if not an automated deployment directly to the hardware.
###### 24. How does the *[Product Training](/docs/elements/producttraining/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
How your team trains people using your solution has no impact on your team's ability to implement continuous integration.
###### 25. How does the *[Support](/docs/elements/support/)* in your context impact the probability that *implementing continuous integration* will add value to your process?
How your team supports people using your solution has no impact on your team's ability to implement continuous integration.

