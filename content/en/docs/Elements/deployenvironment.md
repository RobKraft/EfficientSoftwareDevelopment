---
title: "23. Deployment Environment"
description: "Where is your software deployed to?  Web sites, phone apps, desktop apps, or somewhere else?"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 230
---

###### Deployment Environment
Software solutions are deployed to many different environments, most notably as web applications, desktop applications, through app stores, or embedded in hardware devices.  The different deployment destinations affect some software practices and render others completely useless.  Most notably, perhaps, is that Continuous Deployment (the “CD” of “CI/CD”) is impossible for most, perhaps all, software embedded on devices such as watches or airplanes.  A JamStack deploy through a hosted product such as Netlify likely looks much different than the deployment of a REST API to an on-premise server that has a relational database on the back end.  Deployments in complex environments with many integrated solutions require more coordination between teams and probably influences project selection and scheduling priorities and with the status reporting requirements and integration testing needs of the solutions.
