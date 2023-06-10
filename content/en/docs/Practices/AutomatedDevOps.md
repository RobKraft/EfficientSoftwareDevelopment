---
title: "Automated DevOps"
description: "Considerations of how your context impacts your ability to gain value from DevOps Automation"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 40
---

### What is DevOps Automation?
With the exception of software that is coded and developed directly where it is deployed and used (such as in many low-code environments), action is required to take the "completed" code and deploy it to a location where it executes and is used by clients, customers, staff, employees, the public, and others.  The process of deploying the software can loosely be referred to as your "developer operations", aka "DevOps".  Frequently when we use the word DevOps we are referring to tools that automatically handle some or all of the deployment steps for us, but it is important to realize that in most contexts, every step is not 100% automated.  A few steps may remain manual.  But there has certainly been a strong and popular trend in the majority of development shops this century to automate deployment.

### Why implement automated DevOps?
Automated deployments usually provide a number of benefits:
* Deployment because less tedious for those involved
* It becomes quicker to deploy
* Deployment is consistent and less prone to bugs since automation does everything the exact same way every time, where humans might miss a step
* Credentials in production are often more secure because they can be pulled in by automated processes from encrypted sources
* Credentials used in test environments and other places throughout the deployment process can become more secure
* Credentials become easier to manage in automated environments
* It becomes easier to set up a new environment, such as deploy to a new server, since much of the deployment is automated
* There is often a record, a history, of the deployment since much of it needs to be configured and changes to the configurations can be tracked
* Developers are happier because they don't have to deal with the tedium of deployment.  IT Staff are happier for the same reasons.
* Deployments to test and QA environments can occur more quickly leading to faster feedback on testing results
* Tests can run against code as soon as code is committed to check for errors, to make sure it passes all written tests, for security vulnerabilities, and for many other reasons.

### Why not implement automated DevOps?
It is difficult to find reasons against making some deployment operations automated.  There are many reasons why you might not want to automate one hundred percent, meaning that every code commit automatically gets pushed to production if it passes all tests.  But automated builds and automating the running of unit tests are easy and extremely valuable in almost every context where they are possible.

* Because there are separate sections for CI, CD, and CI/CD to Prod, this section will focus on the value of automating builds and the running of tests.


### How does your context affect the success you will have with automating Builds and the running of tests?
###### 1. How does the *[Organizational Structure](/docs/elements/orgstructure/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
How your organization is structured has no impact on your team's ability to automate builds and the running of tests.
###### 2. How does the *[Development Team Culture](/docs/elements/devculture/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
Only a dysfunctional culture, very resistant to change with individuals unwilling to share what they know for fear of losing their jobs (once others can do what they do) is likely to oppose automating builds, or automating the running of tests if the team has them.
###### 3. How does the *[Hiring Process](/docs/elements/hiringprocess/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
Your organization's hiring process has no impact on your team's ability to automate builds and the running of tests.
###### 4. How does the *[Team Composition](/docs/elements/teamcomposition/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
Your team's composition has no impact on your team's ability to automate builds and the running of tests, other than the potential lack of knowledge about how to get started and make it happen that many experienced developers can provide.
###### 5. How does the *[Training Provided on Code](/docs/elements/trainingoncoding/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The training your organization provides on code languages and tools has a small impact on your team's ability to automate builds and the running of tests.  If your company wants this automation, the company will hopefully allow the developers to be trained to do it with their tools.
###### 6. How does the *[Training Provided on 'Our Ways of Doing Things'](/docs/elements/trainingonourways/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The training your team provides on your way of doing things has no impact on your team's ability to automate builds and the running of tests.
###### 7. How does the *[Environment](/docs/elements/environment/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The environment your developers have to write and debug code is sufficient to automate builds and the running of tests.
###### 8. How does the *[Project Selection](/docs/elements/projectselection/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The way in which projects are selected has no impact on your team's ability to automate builds and the running of tests.
###### *9. How does the *[Solution Purpose](/docs/elements/solutionpurpose/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
One of the few factors that affects the value of automating builds and running of tests is the purpose of the solution.  If you are building a temporary solution, something that will be used once and will be completed soon, then automated the build and unit tests, if you have any, may not be worth the time.  Prototypes, demo applications, technical proofs of concept, and solutions that produce a single report or output and are then discarded may not benefit from automated builds.
###### 10. How do the *[Application Architecture Priorities](/docs/elements/apparchpriorities/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
Your application's architecture priorities has no impact on your team's ability to automate builds and the running of tests
###### 11. How do the *[Security Demands](/docs/elements/securitydemands/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The security demands of your solution have no impact on your team's ability to automate builds and the running of tests.
###### 12. How do the *[Requirements, Features, and Priorities](/docs/elements/rqmtsandfeatures/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The way your team manages requirements, features, and priorities has no impact on your team's ability to automate builds and the running of tests
###### 13. How do the *[Regulations](/docs/elements/regulations/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The regulations your organization must comply with has no impact on your team's ability to automate builds and the running of tests.
###### 14. How does *[Who Decides What To Do](/docs/elements/whodecides/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
Who decides what to do next on your teams has no impact on your team's ability to automate builds and the running of tests.
###### 15. How does *[Project Management](/docs/elements/projectmanagement/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
How your team manages projects and tasks has no impact on your team's ability to automate builds and the running of tests.
###### 16. How do the *[Quality Processes](/docs/elements/qualityprocesses/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The processes you use to insure quality in your application have no impact on your team's ability to automate builds and the running of tests.  But the automation of your builds and regular running of tests can provide a lot of improvement in quality to your solution.
###### 17. How does the *[Architecture Forecasting](/docs/elements/architectureforecasting/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The plans you have for evolving the architecture of your application have no impact on your team's ability to automate builds and the running of tests.
###### 18. How do your *[DevOps](/docs/elements/devops/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
Your current DevOps processes have no impact on your team's ability to automate builds and the running of tests, unless perhaps you have an employee whose sole responsibility is to run builds and tests, and this employee will be out of a job once this is completed.
###### 19. How does the *[Architecture](/docs/elements/architecture/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The architecture of your application has no impact on your team's ability to automate builds and the running of tests
###### *20. How does the *[Code](/docs/elements/code/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
Some types of coding don't have build processes, such as low-code environments or Visual Basic macro script inside of Microsoft Excel.  And some other languages, particularly scripting languages, don't need to be built, but some developers do execute them in test environments against a set of tests after the code is committed to a repo.
###### *21. How does the *[Code Quality](/docs/elements/codequality/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
Code quality can affect your ability to perform automated builds.  When code quality is really bad, specifically when you have many programs that depend on each other in what is known as circular references, you may find it very challenging to automate such a build.  But if it can be done manually it can be automated.  So in some cases that automated build sequence may be: Build Project A, Build Project B, Build Project C, Build Project A again, Build Project B again, etc.  Ideally a team would first attempt to eliminate the circular references, then create a build process that is more straight forward:  Build Project A, Build Project B, Build Project C.
###### 22. How does the *[Application Quality](/docs/elements/appquality/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The current quality of your application has no impact on your team's ability to automate builds and the running of tests.
###### 23. How does the *[Deployment Environment](/docs/elements/deployenvironment/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
The environment into which your software is deployed may have some impact on your ability to automate builds and tests, primarily because the environments don't support builds or unit tests.  Some examples include scripting languages, low-code environment, and Excel macros.  Other examples are software written that talks directly to physical devices such as phones, GPS devices, and Arduino controllers.  However, many of the most popular languages and hardware devices that you can write software for also have emulators/simulators that allow you to deploy code to a simulated environment for testing, and you may be able to add some automation there, if not an automated deployment directly to the hardware.
###### 24. How does the *[Product Training](/docs/elements/producttraining/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
How your team trains people using your solution has no impact on your team's ability to automate builds and the running of tests.
###### 25. How does the *[Support](/docs/elements/support/)* in your context impact the probability that *automating builds and the running of tests* will add value to your process?
How your team supports people using your solution has no impact on your team's ability to automate builds and the running of tests.
