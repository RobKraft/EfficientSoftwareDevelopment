---
title: "9. Solution Purpose"
description: "Is the software mission critical to the business?  Do lives depend on it?  Is it an internal app with little impact if flawed?"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 90
---

### Solution Purpose
One aspect of software development teams that produces a large variance in which practices work best compared to other software development teams is the people that will use the software.  For some teams, solutions are used by other employees in the company.  Some teams write software that gets deployed and used by a group of paying customers.  Some teams write software for use by the general public.  Some teams write software that is used by a single client.  Some teams write software that is only used for a few months then discarded.  Some teams write mission critical software that keeps a business running.  Some teams write software for internal use by the company but the software is not critical and used only occasionally.  In each of these different contexts, that which constitutes a best practice is likely to be different, yet these are all teams developing software.
In addition to the general differences in solution purpose between companies, the purpose of solutions within a company may deviate from their normal purpose.  When developers need to experiment with a new programming language or technology, it may be best to expect that some of the usual processes followed during the SDLC are altered.  The same is true when an application is a prototype, or when a junior developer is learning a new technology.  In some of these cases you may choose to forgo unit tests, secondary code reviews, security audits, or robust documentation, because such actions add waste to the process.

An application that is just a proof of concept or demo or just to learn a new technology should be developed differently than one that is core to our business.  If we followed our most stringent processes for every solution/project, we may often be incurring waste of time on things that add no value.

##### What is the intended purpose of the solution in your context?
1. **Core Internal Business Solution**  
   - *Purpose*: Optimize key internal operations (e.g., ERP, accounting systems).

2. **Commercial Software Product**  
   - *Purpose*: Generate revenue by selling software to customers (e.g., QuickBooks, Microsoft Office).

3. **Revenue-Generating Online Platform**  
   - *Purpose*: Provide a service to users and generate revenue via online platforms (e.g., Amazon, Facebook.com).

4. **Deployed Mobile or Web App**  
   - *Purpose*: Deliver functionality through app stores or web access (e.g., Facebook app, GMail).

5. **Embedded Software**  
   - *Purpose*: Operate or control physical hardware (e.g., car software, GPS firmware).

6. **Minor Internal Business Tool**  
   - *Purpose*: Support small-scale or department-specific tasks (e.g., tracking equipment or schedules).

7. **Client-Owned Custom Software**  
   - *Purpose*: Fulfill a client's request for a custom-built solution they will own.

8. **Disposable Solution for a Specific Task**  
   - *Purpose*: Solve a single-use problem or provide insights, then discard (e.g., data analysis scripts).

9. **Prototype**  
   - *Purpose*: Test market interest with a basic version of the solution.

10. **Proof of Concept**  
    - *Purpose*: Demonstrate feasibility or validate a technology or approach.

11. **Learning Tool**  
    - *Purpose*: Enable developers to practice and gain skills for future projects.


##### How Purpose Affects Practices
* Testing rigor
* Documentation depth
* Security requirements
* Deployment frequency
* Architecture choices

##### Anti‑Patterns
* Treating prototypes like production systems
* Over‑engineering disposable tools
* Under‑engineering mission‑critical systems

##### Templates
* Purpose classification worksheet
* “Right‑sized process” decision tree
* Risk profile matrix