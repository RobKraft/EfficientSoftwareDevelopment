---
title: "11. Security Demands"
description: "How important is security for both the product and the process?"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 110
---

###### Security Demands
Software is used in almost everything of material value in our world today, and it is relied upon to protect that value against a world of hackers and adversaries that desire to cause harm.  The value of items protected by some software solutions is much different than the value of items protected by others.  Therefore, software developers benefit from different levels of controls, practices, and processes used during software development and in the resulting solution based on the value of the items the software may allow access to.  Software must correctly identify the user and determine their appropriate level of permissions.  Software must protect sensitive data collected from exposure.  Software must not allow unauthorized agents the ability to control machines and manipulate data.  Many of the protective measures are part of the software solution itself, but some controls must also be in place during the process of software development to prevent abuse.  The level of controls both within the software, and in the software development processes, varies across software solutions and needs to be evaluated for each solution to avoid the waste produced by implementing excessive security controls where they are not needed.

As the security demands increase, so do the resources and time required increase, often exponentially.  Grandma's recipe application should not be developed with the same security processes as the software storing secret nuclear codes because that would create a lot of time wasted for the development of Grandma's app.
##### How important is security in your context?
* A phone app or website for a bank
* A phone app or website for bank employees with access to all client accounts
* A phone app that is a free game with no way to accept payments, such as solitaire
* An internal accounting application for a small business
* A payroll application for a large company
* An internal application for scheduling games in the teams internal pickleball league

##### How important are these security demands?
* Insuring people logging in are who they claim to be?  MFA
* Protecting users financial secrets such as credit card numbers?
* Protecting users logon ID's and passwords?
* Managing users Personally Identifiable Information (PII)?  GDPR compliance
* Tracking which users made which changes to sensitive data?
* Tracking which users viewed which documents?
* Encrypting all password credentials on production servers?
* Keeping sensitive production data out of test systems?
* Encrypting backups of all production data at all times?
* Encrypting all traffic on your internal computer network?
* Automating all credential management throughout the DevOps process?
