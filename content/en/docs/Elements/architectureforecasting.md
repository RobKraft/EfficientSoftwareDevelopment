---
title: "17. Architecture Forecasting"
description: "What plans and actions are you taking to keep your software product working in the future?"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 170
---

### Architecture Forecasting
The timely delivery of software solutions depends a lot on the execution of the developers.  This puts pressure on developers, often directly from those they report to, to focus on doing things to speed up delivery and improve quality.  This leads many developers to invest little or no time in analyzing the future.  As an analogy, developers are focused on building a quality road quickly through the forest, without lifting their heads above the trees to see if the road they are building is heading in the right direction.  It is not only lack of time for such considerations, but also lack of motivation to do so in companies where morale is low, or lack of time to consider the larger picture for junior developers and developers new to a project that are overwhelmed trying to understand the current state of the software and its processes for development.  When teams look toward the future, they often identify new technologies that their solutions will need to support.  They recognize they need to keep evolving their solution to newer versions of frameworks and languages upon which they are based.  Gradually adopting new versions of the dependencies upon which solutions are based allows the software to exist longer because teams aren’t faced with making substantially large alterations to the software over a short time period to adopt the latest version of the frameworks they depend upon.  Large alterations also incur more risk than a series of small alterations spread out over a long time.  The challenge and risk of upgrading to the newer version of a dependency that is many versions beyond the one currently in use prevents some teams from making the change and may force their customers to continue using older technology that lacks security fixes and performance improvements.  A few specific examples may be helpful to clarify the value of architecture forecasting:
* Many software solutions have migrated to the cloud, and for many, one change made to the application is to use OAuth instead of a simple logon/password combination for authentication.  Changing the logon mechanism is just one of many changes some applications must make to run in the cloud.  However, the change is one that can probably be made in the on-premise version of the application before the other changes that are necessary for the cloud version.  By making the switch to OAuth with the on-premise version, the team removes one big piece of the change prior to their cloud migration.  This also allows the OAuth change to be tested independently, any problems caused by bugs introduced are not obscured by all the other changes in the application that could have caused the bug.
* A company may decide to migrate their solution based on Microsoft’s .Net technologies to the latest versions (.Net Core) in order to run faster and on less expensive cloud servers.  If the current solution is using the WCF technology, the team will need to change the solution to use WebAPI, then migrate it to the .Net Core version of .Net API.  With good technology forecasting, the team could recognize the need to make changes to the dependencies used by the application to support the future ability to run on .Net Core, and start making small incremental changes regularly to achieve that goal.  This reduces the massive amount of work that will otherwise be necessary to convert the app based on WCF to one that works on the latest version of .Net Core.  The biggest benefit of small incremental changes may be that the risk and bug resolution is spread out over a long time, but another benefit may be the possibility of new capabilities.  In this example, by changing the application to run on .Net Core the application also is more likely to be able to run on the Linux OS instead of the Windows OS.  And from the previous example, by moving the application from on-premise to the cloud, integration with other software suites providing features may become available.  It may become easier to integrate with a document signing service, or to scale the resources of the application based on usage, or to monitor the health and status of the application, or to integrate with social media platforms securely.
Making small changes to the application to use current versions of dependencies:
* Allows developers to take advantage of developer productivity features in the dependencies sooner.
* Allows the application to take advantage of new features provided by the update.
* Implements fixes and improvements to security and performance that often come in updates.
* Spreads the risk caused by breaking changes across many minor updates instead of a single large cumulative jump which makes the resolution of problems related to the changes easier to detect and quicker to remedy.
* Reduces the chance that the team’s schedule for delivery of new features is not delayed due to the need to adopt a more current version of the dependency because the newer version has something, such as a security patch or support for a new operating system.
Many organizations find this element challenging to adopt and realize when agile teams focus on the short term goals of providing value to the customer with each product delivery.  Some teams that adopt OKRs based on company goals are unable to approve the implementation of small, incremental framework changes because the changes can’t be shown to add value to customers or to the company goals in the upcoming quarter or year.
Although this section is already lengthy, the most valuable aspects of forecasting are probably related to forecasting how your solution will change and the evolution of technologies external to your solution that  may eventually affect your solution.  In order to adopt the new technologies emerging your application probably needs to keep dependencies up to date, but also be designed and architected to be open to implementing new technologies, tools, and frameworks as they emerge.  More importantly, teams that are aware of what is coming in the future can avoid writing code in the present that will be incompatible with those new technologies and feature requirements when it comes time to develop and use them.


##### How does your development team plan to evolve the architecture of the solution for the future in your context?
* We don't, we expect our solution to reach its end of life soon.
* One or more developers on our team pay attention to the changing trends and new technologies and we begin evolving our software to adapt more easily to the changes we plan to adopt.
* Marketing teams and product owners let us know what new technologies they want to adopt.  Until we get a request from them, we don't think about it.
* We strive to keep our existing tools, frameworks, SDKs, and dependencies current to take advantage of new functionality and to better transition to future changes.
* We don't take time, or don't have time, to invest in updating our existing tools and frameworks.  As long as they meet our immediate needs we will use them as is.


##### Forecasting Techniques
* Architecture runway
* Technical radar
* Scenario planning
* Capacity modeling

##### Good Practices
* Regular architecture reviews
* Incremental evolution
* Tracking emerging risks
* Aligning architecture with product strategy

##### Anti‑Patterns
* Big‑up‑front architecture
* No forecasting at all
* Ignoring tech debt trends
* Architecture disconnected from roadmap

##### Templates
* Architecture forecast report
* Tech radar template
* Risk horizon map