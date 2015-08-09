---
layout: post
title: How to not practice TDD
---

Here are a few rules I’ve learned to follow when practicing test driven development (TDD):

### Don’t use a common dataset that all tests end up using.

 * If you have to make a change to that dataset to accommodate for a new test, it might end up breaking all of your other tests in the process.

## Unit testing is usually good, but not if what you’re testing is changing every 2 days.

 * If the API for a set of functions or a class is changing every day or so and you’re frantically trying to re-write your tests to reflect the API changes, then you might be spending too much time on testing. It’s ok if you initially spend just as long writing tests as you spend writing the functions/methods themselves, but if the specification changes really frequently, you’ll end up frantically trying to re-write your tests before you can get on with the functions themselves.

## Don’t refactor it before you test it.

 * The idea with TDD is that you design your functions by testing them first. Refactoring comes in after the tests, when you re-write the guts of it to be more readable to other developers, faster, more concise, etc. Prematurely optimizing or refactoring code usually leads to accidentally changing how the function works, and if you haven’t finished tests for that then it’s harder to spot the error.

## Don’t write 500 assertions per test.

 * Ok, I might be exaggerating just a tad, but if you write a test with 500 assertions in it, it should be pretty obvious to you that you’re trying to test too much in one function. Break it up for readability and maintainability.

Like all software development practices, there’s a time and a place for TDD. Make sure to look before you leap; if TDD won’t end up saving you time or increasing your productivity, then it’s probably not worth it.
