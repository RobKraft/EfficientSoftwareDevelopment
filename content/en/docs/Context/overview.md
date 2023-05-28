---
title: "0. Overview of Software Context"
description: "All the things that impact your process for delivering software."
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 1
---

Ask a consultant for the solution to a problem and the most likely answer is, "It depends."  This is a fair and honest response that reflects the reality that the best solution to a problem in one context may not be the best solution for a similar problem in another context.

But what is meant by context?  A context is the collection of elements that may affect the success of a change you introduce.  In software development, context includes the software architecture, the experience level of the development team, the processes used to manage projects, the environment into which the software is deployed, and more.  Each of the elements of the software development context may have some impact on a team’s ability to successfully implement a new practice into their environment.

An example of a new practice you could consider is Test Driven Development (TDD).  Some software development teams use TDD and accrue a lot of benefit.  But will it benefit your team?  The answer is, "It depends".  It depends upon your software development context.  If your developers are primarily modifying an existing codebase, especially in an environment that doesn't support unit tests, then TDD may not be practical for your team.

Another example is the practice of Continuous Deployment.  A lot of teams that deploy web sites love the ability to continuously deploy bug fixes and new features to production automatically as they check code changes into the repository.  But a team creating phone apps to deploy to an app store may find that continuous deployment is not an option.

These two examples are cases where it is obvious the new practice won't work, but many practices will not work in some environments for more subtle reasons.  For example, a team may be writing new code for Extract, Transform, and Load (ETL) processes.  The team may consider using TDD but discover the TDD practice leads to wasting too much time writing and rewriting tests that primarily mock calls to databases and offer little assurance that the code will work even if it passes those tests.

Context matters!  Don't assume that a practice providing great benefits in one context will be just as successful in other contexts.  You have probably read articles or heard presenters touting the benefits of practices such as Scrum, TDD, Pair Programming, or Continuous Delivery; and declaring that all software developers should use these practices.  Don't fall for it!  Be a little skeptical!  Learn more about the practice and consider your context to decide if it is right for you to try.  If you try the practice and it doesn’t work, that doesn’t necessarily mean you are doing it poorly, it may mean that the practice is not right for your context.  If you really want to use the practice, you may be able to make it successful by changing other elements in your context first.

[Original post](https://csharpdeveloper.wordpress.com/2021/11/30/context-will-determine-if-a-software-practice-is-right-for-your-team/) 