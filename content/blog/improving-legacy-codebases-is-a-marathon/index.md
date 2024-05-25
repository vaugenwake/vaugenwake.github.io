---
title: "Improving a legacy codebases is a marathon not a sprint"
date: 2024-05-25
description: "This is a description"
tags: ["Tech Thoughts"]
showSummary: false
---

I have a very weird and strange hobby, I like fixing and cleaning up old, crusty and aging codebases with new shinny implementations.

I find joy in trying to bring an old codebase back from the bring of complete destruction and giving order back to chaose. Old codebases have something you can't find in a new fresh greenfield codebase.... Personality.

I have found so much enjoyment from this strange hobby I thought I would detail some of my moniset when I tackle a codebase clean up and the mental pattern I hold when tackling a new challenge.

## Find joy in the process of discovery and question everything
If you are going to embark on a journey to try and rescue a codebase you need to understand two things:
* Why does this thing exist?
* What is the real intention of this existing, what are we solving by this being here?

Before I change anything I will read the codebase. No not every line... but the headlines, the most important parts, the bits that really matter. I will understand why the world looks the way it does, why did the perosn who wrote this code do this.

When you understand why something exists and the intentions behind it, you can begin to deconstruct is core building blocks.

## Start small, get more bold as you go
I see this all the time when developers get "inspired" to clean up a codebase. They get a massive paint brush (IDE) and start to paint the town red with 10,000 line pull-requests expecting their peers to say:
> Oh, your a legend! Lets get this merged in on this Friday afternoon at 4pm

If you couldn't guess, I believe in starting with minor small changes. I will always start with a minor improvement, a class here, a mehtod there and see how I feel about the changes I am making.

As I grow in confidence and understanding in what vision I am trying to create I will begin to get bolder. Rewritting complete features, implementing new features, deprecating methods etc.

As a get more confident and change more items, I will often begin to understand the reason something exists the way it does and being to start asking myself questions about if I should change it, or just simply give is a bit of an edit and a sanity check.

## Everything can be tested, even when you think it can't be
Look, I don't believe that test solve all development errors and things never go wrong, but if you want confidence in your changes then test are really a great way to demonstrate in your pull-requests that your changes are valid and working.

**Testing strategy for older codebases:**
1. Add a test for the current implementation
2. Merge test for current implementation
3. Update implementation and related test
4. Merge updated version

Now you have solved two things:
1. You have a test documenting the intended purpose of your new code
2. Improved the ability for someone to work on this codebase in the future

## Have a close group of collaborators
I am lucky to have a close group of collaborators who help me sort through my proposed changes. Having a community of individuals who challenge your assumptions and ensure you are making a valid change is invaluable in the process of trying to improve a codebase.

Have a group of like minded individuals allow you to:
1. Consult a group of experts when you get stuck
2. Test proposed changes by asking people for feedback before you go to far

You collaborators should not just be "Yes men". They should be strongly opinioned in their own right's and be individuals who's work you respect and admire. You should be able to learn from their feedback and in turn, do the same for them. Having this group around you makes motivating your changes easier, especially if they start to get quite large.

## Closing thoughts
Throwing a codebase aways and starting completely fresh is not always the wrong move. However, it is often the solution most developer are far to quick to reach for as it seems like the quickest and easiest root to a better future.

I believe this action highlights a lack of quality and standards. Unless you tackle the reasons the codebase got the way it did, you are almost certainly end up back there you started in your new shiny codebase.

Cleaning up old codebases will improve your ability as a developer to debug, problem-solve, investigate bugs and improve your competence in motivating your PRs through code review. It is not the easy thing to do, but it is the most valuable learning exercise you can do to grow your skill and get yourself noticed.