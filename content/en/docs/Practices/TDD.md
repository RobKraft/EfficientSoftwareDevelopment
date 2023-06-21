---
title: "2. Test-Driven Development (TDD)"
description: "Considerations of how your context impacts your ability to gain value from test-driven development"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 20
---

### What is test driven development (TDD)?
Test-driven development is the practice of writing tests to specify the requirements, then writing the code to pass the tests.  Because code blocks must be small to pass tests, the code evolves from a set of correctly coded small functions into the solution set needed to complete the full feature specified.  [Link to test-driven development on wikipedia](https://en.wikipedia.org/wiki/Test-driven_development).  Many teams write code first and tests later, but studies show that teams are more likely to end up with tests when they write the tests first.

### Why adopt TDD?
Given that tests can be written before or after coding, many point out that TDD is not really about having a suite of tests, it has other advantages.  First, while a developer is coding they are less afraid of inadvertently breaking existing code when they know all existing use cases are covered by tests.  Second, code written using TDD is more likely to be written in a testable way, and more likely to follow contract patterns than could be defined and abstracted in the code.  In short, the code design is often better and easier to maintain and enhance.  

### Why not adopt TDD?
There are a few potential drawbacks to using TDD.  It may add little or no value for senior developers that can already visualize the end result that is needed.  It also may take more time as many tests may need to be rewritten when developers identify better abstractions and patterns to use while writing code.
Finally, there are many situations in which TDD is not very practical, such as on software languages that lack tooling to support tests.  Also it can be more effort than it is worth to begin writing tests for an existing large code base that currently has none.  Third, many tests may add little value because they are extremely similar to other tests already in the suite or because the code tested is so simplistic that it will never be incorrect; which means developers are wasting time writing tests if there is some other task that could provide more value to the organization.  Finally, some tests that would be most valuable require a lot of data preparation and mocking tools, but these tests, referred to as regression tests or integration tests, are usually not part of the TDD development flow and should not impact your consideration of the value of TDD.

TDD not be very helpful on many maintenance changes, renames in code, and refactoring when you already know what change needs to be made.  It also can be difficult to apply when evolving code to new frameworks and classes, or when making performance improvements or security improvements.  Some features of the code make the TDD approach more work than value obtained from TDD.


The considerations below are provided regarding the process of TDD specifically, not the value and merit of the tests themselves.

### How does your context affect the success you will have with TDD?
###### 1. How does the *[Organizational Structure](/docs/elements/orgstructure/)* in your context impact the probability that *TDD* will add value to your process?
How your organization is structured probably has no impact on your team's ability to use TDD.
###### 2. How does the *[Development Team Culture](/docs/elements/devculture/)* in your context impact the probability that *TDD* will add value to your process?
As with any practice, people will be more willing to adopt it or try something new when they are in an environment that fosters experimentation, openness, and growth.  Otherwise, the team culture is unlikely to have much impact on your team's ability to use TDD.
###### 3. How does the *[Hiring Process](/docs/elements/hiringprocess/)* in your context impact the probability that *TDD* will add value to your process?
Your organization's hiring process probably has little impact on your team's ability to use TDD.
###### *4. How does the *[Team Composition](/docs/elements/teamcomposition/)* in your context impact the probability that *TDD* will add value to your process?
Junior developers, or those new to a new coding language, are probably most likely to benefit from TDD because it can help them learn to solve problems in small steps and in a manner that usually results in composable, robust code.  Senior developers may benefit less from TDD, especially when they can visualize the end goal before they start coding and can write it on their first attempt, without going through iterations to get there.
###### *5. How does the *[Training Provided on Code](/docs/elements/trainingoncoding/)* in your context impact the probability that *TDD* will add value to your process?
Developers with little formal training on how to write and structure code well, especially code that is part of large code-bases worked on by many developers, can probably derive a lot of benefit from using TDD.  Once they understand the IDE and tooling and the basics of the language, they can use TDD to write code that is more clean and SOLID and robust.  
###### *6. How does the *[Training Provided on 'Our Ways of Doing Things'](/docs/elements/trainingonourways/)* in your context impact the probability that *TDD* will add value to your process?
Whether or not you train your new developers on your ways of doing things probably has little impact on your new team member's ability to use TDD, unless your ways of doing things specifically require TDD.
###### *7. How does the *[Environment](/docs/elements/environment/)* in your context impact the probability that *TDD* will add value to your process?
The environment is a very important element in the ability to succeed using TDD.  Some development environments don't support it at all.  Some examples of that include the low-code environments, and a lot of older technologies that don't include testing tools in the IDE's such as Microsoft Visual Basic, DBase, most SQL coding languages, Office Basic, and many more.  TDD requires tools and IDEs with testing features.  Mocking features in the testing tools are necessary in most cases also.  In some cases, more CPU may be beneficial to run large suites of tests quickly.
###### 8. How does the *[Project Selection](/docs/elements/projectselection/)* in your context impact the probability that *TDD* will add value to your process?
The way in which projects are selected probably has no impact on the success of TDD, though some projects, such as new development, may better facilitate the use of TDD.
###### *9. How does the *[Solution Purpose](/docs/elements/solutionpurpose/)* in your context impact the probability that *TDD* will add value to your process?
Reminder, TDD is not about producing tests.  Some solutions don't need or even desire tests.  Prototypes, demo apps, technical proofs of concept, integration scripts, run once projects,  and solutions that are temporary often don't merit the time required to produce tests to go with them.  Getting a solution deployed quickly may be more important than having any tests for the solution.  Solutions where the damage caused by errors and the ease of fixing errors is minimal benefit less from tests.  Yet in some of these cases, the TDD process may help produce the solution even if the tests are discarded.  If quality is not important, and the solution has a short lifetime, TDD and tests probably provide less value.
###### 10. How do the *[Application Architecture Priorities](/docs/elements/apparchpriorities/)* in your context impact the probability that *TDD* will add value to your process?
The benefits TDD may provide probably do not vary much even if your application places strong demands on performance, or scalability, or back-compatibility, ore most other architecture priorities.  Tests can make a very big difference, but the TDD process itself probably does not.  One exception to this may be if your architecture needs a robust API, because APIs consumed by others usually demand higher reliability, predictability, along with simplicity.
###### 11. How do the *[Security Demands](/docs/elements/securitydemands/)* in your context impact the probability that *TDD* will add value to your process?
Like other architecture priorities, the security demands of your solution have little impact on your team's ability to use TDD, and TDD doesn't necessarily contribute to the security of your code.
###### *12. How do the *[Requirements, Features, and Priorities](/docs/elements/rqmtsandfeatures/)* in your context impact the probability that *TDD* will add value to your process?
In order to write tests you need to know what results to expect.  You need clarity in your requirements.  Without that, you may spend a lot of time rewriting tests and software as you repeatedly discover that the feature you delivered is not what the users of the feature wanted.  This is not a problem unique with TDD, but it does mean that you are more likely to throw away a lot of tests, and consider the time you spent writing them to be wasted, when you are unable to obtain clear requirements when needed.  The waste is not only unproductive, but can also be demoralizing to team members.  From the opposite perspective, using TDD can help you discover more quickly when your requirements are not complete.  So if you are able to get clarification easily, TDD can be very helpful to getting code right the first time.
###### 13. How do the *[Regulations](/docs/elements/regulations/)* in your context impact the probability that *TDD* will add value to your process?
The regulations your organization must comply with probably have no impact on your team's ability to use TDD.
###### 14. How does *[Who Decides What To Do](/docs/elements/whodecides/)* in your context impact the probability that *TDD* will add value to your process?
Who decides what to do next on your teams probably has little impact on your team's ability to use TDD.
###### 15. How does *[Project Management](/docs/elements/projectmanagement/)* in your context impact the probability that *TDD* will add value to your process?
How your team manages projects and tasks probably has little impact on your team's ability to use TDD.
###### 16. How do the *[Quality Processes](/docs/elements/qualityprocesses/)* in your context impact the probability that *TDD* will add value to your process?
The processes you use to insure quality in your application probably have little impact on your team's ability to use TDD, but TDD may produce higher quality code which simplifies quality assurance processes.  Tests themselves are a quality assurance practice.  Developers write their own tests on some teams, but QA employees write tests for other teams.  TDD tests are almost always written by developers as part of the development process, but those tests can be included with the tests created by the QA team.
###### 17. How does the *[Architecture Forecasting](/docs/elements/architectureforecasting/)* in your context impact the probability that *TDD* will add value to your process?
The plans you have for evolving the architecture of your application probably have no impact on your team's ability to use TDD.
###### 18. How do your *[DevOps](/docs/elements/devops/)* in your context impact the probability that *TDD* will add value to your process?
Your DevOps processes probably don't impact your ability to use TDD, but they may affect your ability to run the tests, particularly if all tests are ran and the test suite is extremely large.
###### *19. How does the *[Architecture](/docs/elements/architecture/)* in your context impact the probability that *TDD* will add value to your process?
The architecture of your application has a big impact on your ability to use TDD.  As mentioned previously, some architectures and partial architectures using low-code solutions offer no tools to write tests.  Microservices may be so small that the pieces of code don't have any logic that needs tests, yet the overall solution does, in which case those would be integration tests, not TDD generated unit tests.  APIs, back-end solutions, solutions without user-interfaces are architectures more likely to benefit from TDD.  Integration scripts and run once projects rarely benefit from TDD.  User Interfaces for web sites, web applications, and phone apps vary in their benefits derived from TDD based on their tooling.
###### *20. How does the *[Code](/docs/elements/code/)* in your context impact the probability that *TDD* will add value to your process?
The specific languages and tools used to write code determine if using TDD is even an option for consideration.  For many older development technologies like Visual Basic 6 or Paradox or FoxPro, unit tests are nearly impossible.  New technologies like low-code IDEs rarely, perhaps never, offer a way to write tests.  If you want to use TDD you certainly need coding languages like C#, Java, Javascript, and many others that support it; along with IDEs that can facilitate the process.
###### *21. How does the *[Code Quality](/docs/elements/codequality/)* in your context impact the probability that *TDD* will add value to your process?
Many developers find themselves unable to get started using TDD because they work on an existing code base that lacks tests, and also because that codebase is not well written and every test to cover the current code would be an integration test because each function in the code does too much.  For poor codebases, much refactoring is probably needed before you can begin making changes to it using TDD as you modify existing features and add new ones.  TDD is much easier to begin with when starting development on a new code base.
###### 22. How does the *[Application Quality](/docs/elements/appquality/)* in your context impact the probability that *TDD* will add value to your process?
The current quality of your application probably has no impact on your team's ability to use TDD.
###### 23. How does the *[Deployment Environment](/docs/elements/deployenvironment/)* in your context impact the probability that *TDD* will add value to your process?
The environment into which your software is deployed may have some impact on your ability to use TDD.  This is primarily because the tooling for some types of solutions and languages is not as easy to write tests with as others.  It is usually easiest to write tests for solutions deployed as back-end processes on servers, and a little more difficult to write tests for solutions deployed in browsers.  Some low-code and no-code platform don't provide any ability to write tests.
###### 24. How does the *[Product Training](/docs/elements/producttraining/)* in your context impact the probability that *TDD* will add value to your process?
How your team trains people using your solution probably has no impact on your team's ability to use TDD.
###### 25. How does the *[Support](/docs/elements/support/)* in your context impact the probability that *TDD* will add value to your process?
How your team supports people using your solution probably has no impact on your team's ability to use TDD.

#### What does ChatGPT think?
(May 2023)Hey ChatGPT: What are good contexts and bad contexts for test driven development?

Test-driven development (TDD) is a software development technique that emphasizes writing automated tests before writing the actual code. While TDD can be a powerful tool for improving software quality and speeding up the development process, there are certain contexts where it may be more or less effective. Here are some examples:

Good contexts for test-driven development:
1. Large, complex projects: If you're working on a large, complex software project, TDD can be a great way to ensure that each piece of code is tested thoroughly and works as intended. This can help catch bugs early in the development process and reduce the likelihood of major issues down the line.
2. Collaborative development: If you're working on a project with multiple developers, TDD can help ensure that everyone is on the same page and that changes to the codebase don't break existing functionality. It can also help with knowledge transfer and collaboration.
3. Critical functionality: If you're working on software that performs a critical function (e.g., financial software), TDD can be a great way to ensure that the software is reliable and performs as expected. This can help prevent costly mistakes and ensure that the software is trustworthy.

Bad contexts for test-driven development:
1. Simple projects: If you're working on a simple software project, TDD may not be necessary. Writing tests for every piece of code can be time-consuming and may not provide significant benefits.
2. Tight deadlines: If you're working on a project with a tight deadline, TDD may not be the best choice. While TDD can help catch bugs early in the development process, it can also be time-consuming and may slow down development.
3. New technology: If you're working with a new technology that you're not familiar with, TDD may not be the best choice. It can be difficult to write tests for code that you don't fully understand, and this can slow down development.

Overall, TDD can be a powerful technique for improving software quality and collaboration, but it's important to consider the specific circumstances of each project before deciding to use it.
