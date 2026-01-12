---
title: "10. Application Architecture Priorities"
description: "What aspects of your software solution are most important?"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 100
---

### Application Architecture Priorities
We want all applications to be secure, fast, easy to use, and full of all the features customers need.  But every solution values one or two of these objectives more than others, and those values influence how the software is developed, and some of the practices that work best in facilitating that goal.  Some software solutions must be as secure as possible to prevent sensitive data leaks or to prevent undesired access to capabilities.  Other software solutions find it more valuable to deliver software quickly than to implement all the possible security features.  

Are we writing software to prevent the asteroid from striking earth in 42 days, or software to store grandma's recipes?  The purpose determines security concerns, scalability needs, performance needs, speed of delivery, tolerance for errors.  These factors, in turn affect processes, architecture, and the practices that will best help us meet our goals.

#### What are the architectural priorities of the solution in your context?
* 100% uptime.  Our solution must never be offline. (911 Call Center software.  Life support system software. Amazon AWS.  Microsoft Azure.)
* Customer satisfaction.  We will do whatever it takes to please the customer(s).
* Ease of use.  Our software needs to be really easy to use by anyone without training or documentation. (Microsoft Word or Google Docs.  Gmail.  Facebook.)
* Fast.  Our software needs to eke out as much computing power as possible when running on the best hardware and networks. (Bitcoin mining)
* Our software needs to process an enormous amount of data quickly. (Netflix streaming)
* Security.  Our application must never be hacked or compromised.  (Banking applications)

##### How critical is your application?  How important is it that you 'get it right'?
* Very low, static content or a game with no ramifications if there are bugs
* Minor errors are probably easily dealt with or resolved.  Very few people impacted.
* Fewer few people use the software but significant financial loss can occur for some errors
* Significant financial loss can occur for significant errors
* Significant loss can occur to our customers or clients if there are errors in our code
* Loss of life can occur