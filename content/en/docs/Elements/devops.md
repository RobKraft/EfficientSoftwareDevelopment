---
title: "18. Automated DevOps"
description: "How automated are your testing and deployment processes?"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 180
---

### Automated DevOps
Writing code is not the last step in delivering a software solution.  After the code is written it must be packaged and deployed, usually with testing and verification that the code meets the requirements.  For small teams, solo developers, and creators of software using languages and tools the developers have never used before, most of the steps in deployment will probably be performed manually.  As teams grow in size and the delivery of solutions because more repetitive companies gain a lot of value by automating steps involved in the deployment.  DevOps is often more than just the steps to deploying the software, but also actions taken to keep the solution running and performing well, and securely, in the deployed environments.  Many steps that follow the writing of the code can be automated to improve consistency, quality, and speed up delivery.  Automation can also be used to provide feedback to developers more quickly about issues, and to ensure code is secure and doing what customers expect it to do.  “Automate Everything” is a philosophy used by some teams, and most teams benefit from automating as much as they can.  The primary reason so teams don’t automate is because the cost of implementing and maintaining the automation is not worth the gain provided.  Beyond the noticeable benefit of speeding up delivery that automation provides, it often improves the morale of developers and I.T. because it alleviates tedious manual tasks they used to perform.  Fast feedback on bugs introduced by developers is also usually appreciated by developers and accepted by them more readily than such negative feedback provided by human testers days or weeks later.  Application quality also can gain significantly through automated logic tests, tests for security vulnerabilities, and automated compliance with auditing and industry regulations.  The DevOps choices a company makes can significantly affect many software development practices because the automations may or may not integrate with those practices, and the tools chosen for automation may not perfectly align with the optimal implementation of some practices.


##### How do you deploy your software?
* The way you deploy your software impacts your options for testing and how you should test and what can be automated.
* We don't deploy, we make low code no code changes directly in the production environment
* We copy files and paste changes into production when/if needed.
* We manually build the artifacts, then copy those files
* We have automated our build process to product output files that we deploy to our production locations.
* We have automated our deployment to copy files and changes files and settings where needed.
* We use a third party tool to build and package what we need to deploy
* We use a third party tool to deploy
* We don't deploy, we just use the code to get results then can discard the code
* We auto build when changes are pushed into a repo
* We auto build on a regular schedule
* We auto deploy to test when changes are pushed into a repo
* We auto deploy to production when changes are pushed into a repo
* We develop software for customers and deployment depends on them


##### DevOps Capabilities
 Continuous integration
* Continuous delivery
* Infrastructure as code
* Monitoring and observability

##### Good Practices
* Automated pipelines
* Shift‑left testing
* Immutable infrastructure
* Blameless postmortems

##### Anti‑Patterns
* Manual deployments
* No monitoring
* Dev vs Ops silos
* “DevOps team” as a silo

##### Templates
* CI/CD pipeline blueprint
* Incident response guide
* Deployment checklist