---
title: "0. Overview of The Elements"
description: "The way people, teams, groups, and departments are organized and work together."
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 1
---

### The Elements of a Software Development Context
{{< img src="/images/elements1-1.png" title="The Elements of Software Development" caption="" alt="image alt" width="700px" position="center" >}}

There is more to software than code.  Software is used to provide a solution to a problem, meet a need, or fulfill a desire.  The goal is to meet that need or solve that problem, not to write code.  Code is just one part of the solution.  Getting the requirements right is another.  Quality assurance processes are important too.  Documentation and support may greatly add to or improve the value of what is delivered.  There are many elements that impact the production of software, and that is what the term elements refers to on this site.  

Elements are all the things that contribute to and affect the software that is eventually delivered.  

The elements are different from one organization to the next.  The elements are often different for teams within the same organization.  The set of elements for a particular software solution can be referred to as the Software Development Context.  The Software Development Context for one solution may use an agile process, while the Context for another solution uses a waterfall process.  The Context for one solution may use the Java language for the code, while the Context for another solution uses C++.  

All of the differences, some minor and some significant, imply that software solutions are developed in different contexts.  This is important to be aware of because it follows from that premise that every software solution may not benefit the same by adopting the same practices and processes.  For decades many software practicioners have looked for practices that greatly improve the efficiency of software development.  Some practices that frequently meet with success are Agile, unit tests, and automated DevOps.  Some that have less adoption are TDD and CI/CD.  The reasons for the success or failure is often not that the practice was implemented poorly, but rather than the practice is just not the right fit for that context.

Much of this site examines the software development contexts hoping to help you realize what practices will work in your context, and what practices won't.

Software Development Contexts vary substantially.  Just as there are few "engineering" best practices, rather there are best practices in each sub-discipline such as "building expansion bridges", "building dams", "building skyscrapers".  Likewise, we should expect different best practices in different software contexts.

[Original post](https://csharpdeveloper.wordpress.com/2021/08/18/the-elements-of-software-development/)
Successful software products and solutions rely on much more than the programming source code put into them.  The elements attempt to identify all the factors that affect the outcome of a software development project.  The value of recognizing each of these elements is to help those involved in a software development process recognize that many elements influence the production of quality software, and each of these elements should be evaluated if you desire to improve your software product and software development processes.

Most people accept, as self-evident, that any process has room for improvement.  The CPI (Continuous Process Improvement) mindset encompasses many programs and frameworks that accept that people can always do better and can systematically attempt to do so.  If you agree that improvement is possible, it follows that you also recognize there are many areas in which improvements can be made.  We can't make all possible improvements simultaneously, therefore we must select a few things to improve and start those before identifying and working on other areas of improvement.

The elements give us places we can look to consider making improvements.  We will find that it is easier to make improvements in some of the elements than in others, but we should also consider which improvements provide the best return on investment (ROI) when undertaken.  We hope practitioners will examine each of the elements and consider if changes could be made that would improve their software development process and product, and direct their energy to those changes that will most likely be successful and provide the best ROI.

{{< alert theme="warning" dir="ltr" >}}
The elements of software development are the things that influence how software is developed.
{{< /alert >}}

Each element has been assigned a category, either Product, or Process, or People.  Elements assigned the people category are elements that affect the development of people.  When you make a change to one of the people elements, you are usually making a change that you hope will improve a person or people.  When people have better training, experience, tools, and workplace satisfaction they are more likely to produce better software.  Elements assigned the process category are elements that are used to produce the product, but that are not present within the product delivered to the client or people that use the product.  Agile methods and DevOps are two very notable elements assigned to the process category that have a significant impact on the successful delivery of a quality product.  Of course the elements of the product category include those things the customers interact with, including training and support along with the quality of the software.
{{< img src="/images/elements2.png" title="Process, Product, and People" caption="" alt="image alt" width="700px" position="center" >}}

{{< alert theme="info" dir="ltr" >}}
On nomenclature:  The word element and category are lower case for a reason.  There is nothing special or significant in the choice of these words.  The word element was selected primarily because it is less used in software literature than many synonyms that could have been used such as component, factor, feature, or module.  Likewise, category is used extensively in the domains of many fields, but in this article it is a simple term used for grouping some similar elements.
{{< /alert >}}


The Software Development Life Cycle (SDLC) has long been considered the list of steps followed for the production of software.  The elements makes no change to that.  The elements identify additional factors that influence how software is produced and that affect the success or failure and quality of the software.  Nine of the elements are noted for having a close correlation in meaning to a step in the SDLC.
{{< alert theme="warning" dir="ltr" >}}
SDLC is the name for the process we use to get from Idea to Solution.
{{< /alert >}}

The first purpose of the elements of software development is to help us identify where we might spend our time to make improvements.  **The second purpose of the elements of software development is to help us identify the current context in which we develop software so that we may make better selection of practices and processes that will lead to success.**  There are hundreds of practices and processes to choose from to use during software development, and much debate about which practices and processes are best.  The truth is that the value of any specific practice or process depends a lot much upon the context in which it occurs.  Perhaps this is best understood from this example:  Some software developers believe strongly in CI/CD and believe that all development teams should make it a goal to deliver software continuously.  However, other software developers work in a context where that is not possible.  For example, continuous delivery of software embedded into gyroscope controllers on a Mars rover craft is impossible.  Even for many contexts where it would be theoretically possible to apply CI/CD, the benefits and risks are not worth the cost of doing so.

**The value of a practice or process must be considered within the context in which it is applied.**  Of the twenty-five elements, all but three contribute to the context in which software is developed.  Therefore, when we consider the use of a different process or practice, we should consider our context as a factor that may make that process or practice successful.  Many software development teams have adopted the Scrum methodology in an attempt to improve their software development.  Unfortunately, the adoption of Scrum has not been successful in every case.  But why is that?  Is it because they are doing Scrum incorrectly, or is it because Scrum is not a good practice for their context?  That is a difficult question to answer.  Unfortunately, a few people dogmatically believe Scrum should always be used by all teams, and that could be based on their own lifetime of experience, which could be all within similar contexts.  These people then may continue to push Scrum even when it is not the best choice in a different context.  This is the outcome we hope to avoid when practitioners consider the context into which they are attempting to apply a practice.

The context for software development for a team reflects the collection of twenty-two of the elements.  The context is the interaction of these twenty-two elements.  The implication is that you should ask if the practice you are considering to adopt is a good practice for your context.  Is it a good practice that aligns with your choices for each of the twenty-two elements that apply to context?  A few examples of processes and practices, Scrum and CI/CD, were already mentioned.  Other examples of processes and practices include Test Driven Development (TDD), Pair Programming, Unit Tests, Automated Builds, Kanban, Retrospectives, Estimates, Metrics, WIP Limits, Story Points, StandUp Meetings.  There are many more.

The hope is that we can use the identified context to make a good selection of practices.  Here is an example that considers just a few of the context elements along with the question, "Should we develop software using TDD?"  If the "Team Composition" is "junior developers", and the "application architecture/design" is "unknown", then asking them to use TDD when they have not done so before may be very valuable to achieving good results.  But if the "Team Composition" is "senior developers", and the "application architecture/design" is "well known", then asking them to use TDD when they have not done so before may be detrimental to the results.  TDD, or any other practice or process, is not inherently always good or bad, but these patterns and practices work better in some contexts than others.

{{< alert theme="warning" dir="ltr" >}}
Context is the collection of factors that influence the choice of best practices for your software development processes.
{{< /alert >}}

The twenty-five elements of software development are used by most software development teams, but not all.  For example, software developed by a single person is unlikely to have a "Hiring Process" element.  However, for each of the twenty-five elements, a software development team made a choice about what to use within each element.  Here are a few examples.  For "Architecture", the choice could be a web application, desktop application, embedded application, or another architecture.  For "Project Management", the choice could be Scrum, Kanban, Waterfall, or another process.  Every software product under development is being developed in a specific context, and that context affects best practices.  Many people probably also understand that the context is rarely static.  A team that is developing an application using one process many also be transitioning to developing the application using a different process.

As mentioned previously, it is probably counter-productive, destructive, or simply impossible to systematically make changes to all the elements of your software development at the same time.  You must select some to begin improving, which means you must choose those that are most valuable to change first.  Even when someone can show you that there is value in changing the way you handle one of the elements, you might not begin making that change because there are more valuable things to focus your efforts on.  The one limiting factor that all software developers share is limited time.

{{< alert theme="warning" dir="ltr" >}}
We have a limited amount of time to spend on creating software and improving processes before the results of our efforts becomes obsolete.  Therefore we must choose wisely how we spend our time.  What changes will produce the most benefit, do the least harm, or introduce the least risk?
{{< /alert >}}
