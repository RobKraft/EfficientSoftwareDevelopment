---
title: "12. Requirements, Features, and Priorities"
description: "How do you gather and manage requirements and features?  How are the most important/valuable items determined?"
date: 2023-05-23T00:00:00+05:00
draft: false
weight: 120
---

### Requirements, Features, and Priorities
Every software solution is brought into existence by the implementation of a succession of features and requirements.  Each solution has its own unique set of features and requirements, but something that varies from one development team to another is how those features and requirements are identified and documented and tracked through the development process.  Some developers understand the requirements better than others.  Some teams acquire a lot of specific details at the beginning while others wait to acquire details until the specific features enter the coding phase.  Some teams talk to end users and customers to get a list of features, other teams make educated guesses about what end users want.  Some teams rarely work with product owners to clarify features under development while on other teams a product owner works with the developers all day long every day to clarify requirements.  Furthermore, teams use different methods to establish the priority, or sequence, in which features and requirements are implemented.  For some teams, the product owner dictates the sequence of features, but for others that is totally controlled by the development team, and of course in many cases the priority is determined jointly by the groups.  
Beyond identifying and prioritizing requirements and features, development teams use different approaches to track the progress of development and also to keep track of when features are provided to customers or end users.  Some software development teams provide little progress information other than perhaps letting the customer know when the feature is available; while others provide daily visualization of the status of the feature and thorough records of when it was delivered.  As with most every element, the correct implementation depends upon many factors in the software development environment.  While it may sound like every team should provide a current status of features under development, such actions could produce waste if no one desires to consume that information regularly.



## 1. Requirements Discovery Practices

Different projects require different mechanisms to learn what to build.

### If requirements are well-known early

- Up-front requirements docs
- Architecture design docs
- Longer release cycles

Work well because the risk is in building correctly, not in discovering needs.

### If requirements emerge late or change often

- Ongoing customer interviews
- Continuous backlog grooming
- Lightweight stories
- Iterative reprioritization

Work well because the risk is in building the right thing, not documenting the wrong thing.

## 2. Prioritization & Decision Authority

Who controls feature sequence determines which planning rituals fit.

### If a product owner dictates priority

- Scrum backlogs and sprint planning align well.

### If developers control priority

- Kanban with technical pull queues or XP-style planning aligns better.

### If priority is negotiated

- Joint mechanisms (OKRs, roadmaps, quarterly planning) help align incentives.

## 3. Feedback & Collaboration Patterns

The level of clarification access influences ceremony needs.

### If developers have constant product access

- Minimal documentation and lightweight tickets suffice.

### If product access is rare

- Heavier specs, acceptance criteria, and validation steps prevent rework.

This is the “communication bandwidth” dimension: low bandwidth → more formal artifacts.

## 4. Progress Tracking & Transparency

Different audiences demand different visibility.

### If stakeholders need frequent status

- Visible Kanban boards
- Burndowns / cumulative flow
- Release notes with timestamps

### If stakeholders don’t monitor progress actively

- Lightweight tracking avoids status reporting waste.


## 5. Waste Avoidance Principle

Don’t add process cost without a consumer.

### Examples of mismatches

- Daily standups with no decisions → waste
- Detailed specs for trivial UI tweaks → waste
- Zero progress visibility for critical clients → friction and distrust

## 6. Practical Implications (Condensed)

To choose practices intelligently, assess three axes:

- **Requirements volatility**
	- Stable → plan more up front
	- Volatile → iterate and learn
- **Decision authority**
	- Clear → optimize flow
	- Shared → optimize alignment
- **Communication bandwidth**
	- High → fewer artifacts
	- Low → more structure

## 7. Multiple Valid Best-Fits (Not one “best practice”)

Different models excel in different conditions:

- **Scrum** — Best when requirements emerge and product owner is available.
- **Kanban** — Best when work varies in size and arrival time, and priority shifts often.
- **SAFe / enterprise planning** — Best when dependencies require synchronized release trains.
- **XP** — Best when customer sits with developers and changes requirements constantly.
- **Waterfall** — Best when requirements are fixed, regulated, or contractual.


##### Anti‑Patterns
* Vague requirements
* “Just build it” directives
* No validation with users
* Requirements that conflict with constraints

---