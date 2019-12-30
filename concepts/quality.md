---
title: Quality
permalink: "/concepts/quality/"
parent: Concepts
---

# Quality in software

Each expression and statement is expressed in code on a spectrum of quality. The overall quality of a system is some aggregation of the individual components and how they are organized.

It takes time to build quality software and it should only be attempted when there is confidence that the software should be used well into the future.

Computers can read code regardless of the quality - it is people who benefit from increased code quality. Beneficiaries include everyone else on your team as well as your future self. Anyone who is going to need to change that code will benefit.

## What is it?

Software that meets business demands today can be incapable of being changed over time to respond to future changes. Quality software meets future business needs - and it builds on software that meet's today's needs as a starting point.

You can change quality software - it is not brittle. Changing something in one area of the code doesn't impact distant functionality.

## How much quality should I want?

If the work is short-lived and not part of the future business, use the least quality possible. Work that may become important is trickier - it is easy to entrench low-quality work causing optional maintenance burdens.
In order to focus on things that matter, we can care the most about things at the top of the stack, relying on tools to enforce standards most completely at the bottom and to a lesser extent further up the stack.

Consistency is important within teams - solving a set of problems with the same solution allows everyone to use the preferred tools expertly.

## How do I measure quality?

 - How much time does the team spend on features vs. bugs
 - How frequently are bugs detected by end-users
 - How much of the functionality is covered by tests that are run before releases
 - Is the application acting surprisingly?

## How do I tune quality going forward?

### The minimum

Prototype the application with available tools so that you can expend the minimum effort to get the job done. If you are forced to write code, do the absolute minimum.

### Medium

Iterate on the application by adding the functionality to the application and than by writing tests. This "should work" for the most part, and it is faster for most people than creating higher quality software.

### High

There are three hats one wears when writing high quality software: red, green, and blue. One always starts with red, then switching to green, then blue, then back to red.

When wearing a red hat, you write a failing spec, thus turning the test suite red. This failing spec should demand the smallest amount of functionality that can be imagined.

After you have a failing spec, the goal is to write the minimum application code to make the test pass (green).

After the test has been written and code updated to allow the test to pass, consider any refactorings that might illicudate your intents.

## How can I tune the quality of existing code?

I have never heard of someone wanting to decrease the quality of existing code, but if you wanted to do that I'd suggest deleting any existing tests. That should do it.

Moving on to the more common goal of improving existing code, the first thing to note is how hard this is to do compared to writing high-quality code from the outset. The reason this path is frought with less quality than new code being written with quality is the difficulty in writing a test suite after-the-fact that covers all of the cases embedded in the code. It is difficult to tease apart everything that would need to be tested but once that is done, writing tests should be straightforward.

Unfortunately the likey result of this "quality backport" is more complicated software than is required to make the tests pass.
