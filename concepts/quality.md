---
parent: Concepts
title: Quality
permalink: /concepts/quality/
---

# Quality in software

Each expression and statement is expressed in code on a spectrum of quality. The overall quality of a system is some aggregation of the individual components and how they are organized.

It takes time to build quality software and it should only be attempted when there is confidence that the software should be used well into the future.

## What is it?

Software that meets business demands today can be incapable of being changed over time to respond to future changes. Quality software meets future business needs - and it builds on software that meet's today's needs as a starting point.

You can change quality software - it is not brittle. Changing something in one area of the code doesn't impact distant functionality.

## How much quality should I want?

If the work is short-lived and not part of the future business, use the least quality possible. Work that may become important is trickier - it is easy to entrench low-quality work causing optional mantainance burdens.
In order to focus on things that matter, we can care the most about things at the top of the stack, relying on tools to enforce standards most completely at the bottom and to a lesster extent further up the stack.

Consistency is important within teams - solving a set of problems with the same solution allows everyone to use the preferred tools expertly.

## How do I measure quality?

 - How much time does the team spend on features vs. bugs
 - How frequently are bugs detected by end-users
 - How much of the functionality is covered by tests that are run before releases
 - Is the application acting surprisingly?

## How do I tune quality?

### The minimum

Prototype the application with available tools so that you can expend the minimum effort to get the job done. If you are forced to write code, do the absolute minimum.

### Medium

Iterate on the application by adding the functionality to the application and than by writing tests. This "should work" for the most part, and it is faster for most people than creating higher quality software.

### High

Iterate very tightly by defining small chunks of work and then writing the smallest test that you can to fail. Continue by making that test pass by adding the application code as required. Next refactor the code and start the PR process.
