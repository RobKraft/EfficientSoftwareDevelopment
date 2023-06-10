---
title: "Continuous Deployment"
description: "Considerations of how your context impacts your ability to gain value from continuous deployment"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 60
---

### What is continuous deployment?
Although there are minor variations to the meaning of continuous deployment, for purposes of this page it means deploying the software to a working test, quality assurance, staging, or other non-production environment every time code is committed and pushed to a shared repository, or on a regular cadence such as every few hours throughout the day.
Many of the elements affecting the automation of continuous integration affect the implementation of continuous deployment in the same way.

### Why implement continuous deployment?
Automating the deployment usually provides three benefits.
* First, it increases the chance the deployment is successful because all the steps and actions that are part of the deployment are automated and thus won't be overlooked or performed out of sequence.
* Second, if deployment are valuable frequently, such as more than a few times per year, it is likely so save time overall to create an automated deployment instead of manually performing the steps every time.  Once the deployment is automated, it can be performed more quickly, sometimes in minutes instead of days.  The deployment can also be performed more frequently, which is often the most valuable benefit.  Instead of spending two days deploying to your test system once a month, you can deploy every night in just a few minutes.  Finally, you should be aware that the people performing the deployment can be freed up to work on other tasks.
* Third, by having quicker and more frequent deployments, testing and quality assurance teams can provide quicker feedback to developers.

### Why not implement continuous deployment?
In some cases, automating a deployment can be difficult.  Some sites deployed to in non-production environments require data for testing, and setting up that data to be suitable for testing may require a lot of work, such as obfuscating sensitive data, changing security data, and removing sensitive production data but replacing it with realistic simulated data.  Many other factors can make it difficult to automate a deployment, so you need to consider if the time required to create the automated deployment is worth the time that will be saved by having it automated.  In some cases, even though you feel it may not be worth the time, when you add in the benefits of being able to deploy more frequently once it is automated, and the benefits of accurately deploying all the steps correctly, you may feel it is worth the effort.  
### How does your context affect the success you will have implementing continuous deployment to a non-production environment?
###### *1. How does the *[Organizational Structure](/docs/elements/orgstructure/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
How your organization is structured may have some impact on your team's ability to implement continuous deployment.  Primarily this could happen if the developer coders are on a different team from the devops implementers and neither team knows a lot about how the other team works.  Getting a good CI/CD pipeline functional requires both developers and people in devops roles working together to make changes to code, configuration, architecture, and processes to get CI/CD working well.  
###### 2. How does the *[Development Team Culture](/docs/elements/devculture/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
Your team culture probably has no impact on your team's ability to implement continuous deployment.
###### 3. How does the *[Hiring Process](/docs/elements/hiringprocess/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
Your organization's hiring process has no impact on your team's ability to implement continuous deployment.
###### 4. How does the *[Team Composition](/docs/elements/teamcomposition/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
Your team's composition has no impact on your team's ability to implement continuous deployment, other than the potential lack of knowledge about how to get started and make it happen that more experienced developers can provide.
###### 5. How does the *[Training Provided on Code](/docs/elements/trainingoncoding/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
The training your organization provides on code languages and tools has a small impact on your team's ability to implement continuous deployment.  If your company wants this automation, the company will hopefully allow the developers to be trained to do it with their tools.  
###### 6. How does the *[Training Provided on 'Our Ways of Doing Things'](/docs/elements/trainingonourways/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
The training your team provides on your way of doing things has no impact on your team's ability to implement continuous deployment.
###### *7. How does the *[Environment](/docs/elements/environment/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
Continuous deployment usually requires an environment that can support many virtual servers that can be built and spun up on demand.  These could be in the cloud or on-premise; either way the organization needs to provide the resources to make all the environments, each of which usually includes their own DBMS and other dependencies.
###### 8. How does the *[Project Selection](/docs/elements/projectselection/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
The way in which projects are selected has no impact on your team's ability to implement continuous deployment.
###### *9. How does the *[Solution Purpose](/docs/elements/solutionpurpose/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
One of the few factors that affects the ability to implement continuous deployment is the purpose of the solution.  If you are building a temporary solution, something that will be used once and will be completed soon, then CI/CD may not be worth the time.  Prototypes, demo applications, technical proofs of concept, and solutions that produce a single report or output and are then discarded may not benefit from CD.
###### 10. How do the *[Application Architecture Priorities](/docs/elements/apparchpriorities/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
Your application's architecture priorities has no impact on your team's ability to implement continuous deployment
###### *11. How do the *[Security Demands](/docs/elements/securitydemands/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?


Security demands of your solution have no impact on your team's ability to implement continuous deployment.


###### 12. How do the *[Requirements, Features, and Priorities](/docs/elements/rqmtsandfeatures/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
Can we overwrite test?
The way your team manages requirements, features, and priorities has no impact on your team's ability to implement continuous deployment


###### 13. How do the *[Regulations](/docs/elements/regulations/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
The regulations your organization must comply with has no impact on your team's ability to implement continuous deployment.
###### 14. How does *[Who Decides What To Do](/docs/elements/whodecides/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
Who decides what to do next on your teams has no impact on your team's ability to implement continuous deployment.
###### 15. How does *[Project Management](/docs/elements/projectmanagement/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
How your team manages projects and tasks has no impact on your team's ability to implement continuous deployment.
###### 16. How do the *[Quality Processes](/docs/elements/qualityprocesses/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
The processes you use to insure quality in your application have no impact on your team's ability to implement continuous deployment.  But continuous deployment and the regular running of tests can provide a lot of improvement in quality to your solution through quicker feedback to developers.
###### 17. How does the *[Architecture Forecasting](/docs/elements/architectureforecasting/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
The plans you have for evolving the architecture of your application have no impact on your team's ability to implement continuous deployment.
###### *18. How do your *[DevOps](/docs/elements/devops/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
The automation of builds can be performed on the same computers developers use to code and debug.  But to implement a CI/CD process with frequent builds and test runs usually requires a separate server to handle the workload so that developers computers aren't slowed down when the processes run, and so that they can build using the code everyone in team has committed, not just the code from one developers computer.  Today, a lot of teams spin up build servers in the cloud to do this.  It can also be done with a traditional server on-premise or in the cloud.  Either way, teams need to be skilled enough to set up and configure the build servers and maintain the build environment, which often also means creating test databases for automated testing processes.  Teams with development based in the cloud generally have an advantage over teams doing all their builds and processes on computers on premise.
###### 19. How does the *[Architecture](/docs/elements/architecture/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?

Seperate teams and microservices, integrations, etc.
The architecture of your application has no impact on your team's ability to implement continuous deployment


###### *20. How does the *[Code](/docs/elements/code/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
Some types of coding don't have build processes, such as low-code environments or Visual Basic macro script inside of Microsoft Excel.  And some other languages, particularly scripting languages, don't need to be built, but some developers do execute them in test environments against a set of tests after the code is committed to a repo.
###### *21. How does the *[Code Quality](/docs/elements/codequality/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
The quality of code in your application has no impact on your team's ability to implement continuous deployment
###### 22. How does the *[Application Quality](/docs/elements/appquality/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
The current quality of your application has no impact on your team's ability to implement continuous deployment.
###### 23. How does the *[Deployment Environment](/docs/elements/deployenvironment/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
The environment into which your software is deployed may have some impact on your ability to implement CD, primarily because the environments don't support builds.  Some examples include scripting languages, low-code environment, and Excel macros.  Other examples are software written that talks directly to physical devices such as phones, GPS devices, and Arduino controllers.  However, many of the most popular languages and hardware devices that you can write software for also have emulators/simulators that allow you to deploy code to a simulated environment for testing, and you may be able to add some automation there, if not an automated deployment directly to the hardware.
###### 24. How does the *[Product Training](/docs/elements/producttraining/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
How your team trains people using your solution has no impact on your team's ability to implement continuous deployment.
###### 25. How does the *[Support](/docs/elements/support/)* in your context impact the probability that *implementing continuous deployment* will add value to your process?
How your team supports people using your solution has no impact on your team's ability to implement continuous deployment.

