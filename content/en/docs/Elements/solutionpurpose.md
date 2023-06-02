---
title: "9. Solution Purpose"
description: "Is the software mission critical to the business?  Do lives depend on it?  Is it an internal app with little impact if flawed?"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 90
---

###### Solution Purpose
One aspect of software development teams that produces a large variance in which practices work best compared to other software development teams is the people that will use the software.  For some teams, solutions are used by other employees in the company.  Some teams write software that gets deployed and used by a group of paying customers.  Some teams write software for use by the general public.  Some teams write software that is used by a single client.  Some teams write software that is only used for a few months then discarded.  Some teams write mission critical software that keeps a business running.  Some teams write software for internal use by the company but the software is not critical and used only occasionally.  In each of these different contexts, that which constitutes a best practice is likely to be different, yet these are all teams developing software.
In addition to the general differences in solution purpose between companies, the purpose of solutions within a company may deviate from their normal purpose.  When developers need to experiment with a new programming language or technology, it may be best to expect that some of the usual processes followed during the SDLC are altered.  The same is true when an application is a prototype, or when a junior developer is learning a new technology.  In some of these cases you may choose to forgo unit tests, secondary code reviews, security audits, or robust documentation, because such actions add waste to the process.

An application that is just a proof of concept or demo or just to learn a new technology should be developed differently than one that is core to our business.  If we followed our most stringent processes for every solution/project, we may often be incurring waste of time on things that add no value.

##### What is the purpose of the solution in your context?
* Core internal business solution (An ERP solution, An Accounting solution)
* Software sold to customers (Quickbooks, Microsoft Office)
* Solution such as a web site used to generate revenue (Facebook.com, Amazon.com)
* An app we deploy to an app store (Facebook, GMail, Stock Trading App)
* Embedded software controlling some hardware (Software in your car, Software in your GPS)
* Minor internal business solution for a few users (Track equipment for the purchasing department, Track vacation schedules for Accounting Department)
* Software requested by a client that the client will own (You are contracted to build a software solution and deliver it by the end of this year)
* Solve a specific problem or answer a specific question then discard it (A python script/program to analyze data, get results, and use for a report)
* A prototype (Build it to see if anyone would be interested in paying for it.  If so, then build a better version of it.)
* A proof of concept (Can we make this technology or idea work for us?)
* To help a developer learn new skills (The little app will help our new developer learn skills to use on our other solutions.)

