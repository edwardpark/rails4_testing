#Rails 4 Testing with RSpec | Cucumber | Capybara

###Why bother with Testing?
###it's slow, not sexy, only matters when it doesn't work

Test Driven and Behavior Driven development is born from this counter-intuitive
idea that developers will be able to improve both the design and
accuracy of code by writing your code test-first.

this isn't suppose to be a full out introduction to the concepts of TDD
and BDD. Instead this is more of the practical application of these concepts
to a project series using the tools RSpec , Capybara and Cucumber.

Things you should know:
[ ] why you are doing this
[ ] what red,green, refactor means
[ ] the idea of what unit testing is.
[ ] add series of prerequistes themselves


### TLDR Introduction
via Matt@GA

As our applications increase in complexity, we need a saftey net. We need something to ensure that we "Do no harm". We need a battery of automated tests. These are specifications about YOUR code that you can run to ensure your code is doing what it should.

Think back to the way you code. You create a part of a web page, then you browse to that page to test it. To ensure that it is doing as you expect. Then you add another feature. And test both features. Then you add a third feature and test... just the third feature. Imagine if you had a battery of automated specs, which run against your code, so you can see if your new changes fit your new requirements and EVERY requirement that came before this.

There a few levels of testing. Acceptance tests verify our apps at the lvel of user interaction. They visit web pages, click on links, validate the DOM. Integration tests check the interaction between objects. Unit tests check the smallest level. The functionality of a specific method.

Sandi Metz (author of POODiR), has a talk titled "The Magic Tricks of Testing".

She discuses that:

Unit tests stand in contrast to integration tests
Unit tests focus on small pieces of code, like single objects
The intent is to ensure the correct functioning of your app at the atomic level
These tests are conducted in isolation, without reference to external objects, as much as possible (using mocks and stubs as placeholders when necessary)
She propounds that our Unit Tests should be:

Thorough
Stable
Fast
Few
They need to be thorough enough to identify an issue at the moment when it occurs. They need to be stable so that we can trust them. No flickering tests. They need to be fast so that we can run all our tests every time we make a change - or we will stop running them. They need to be few so... They need to be few so that... awww, go watch the talk already.

###Testing your Rails 4 applications

So when testing your Rails 4 Application you will be usually using a couple different set to tools

<b>CUCUMBER</b> : This is a tool which allows you to write features that a non-programmer can understand, basic idea
is this it the specs that a client would see so you can talk with them and have their input
<b>CAPYBARA</b> : Allows you to half simulate going through the application and provide what are called end-to-end
integration tests.
<b>RSPEC</b> : this will be the unit tests for you to test the singular modular pieces of code

Ultimately this is going to be a top-level workview down but obviously with time contraints first iteration is going to be a quick
run through each idea of how to write skeleton tests of what you are looking for and then with each iteration add more
details.

[ ] Step 1. Install RSPec , Cucumber , Capybara to your Rails application
TLDR right now read their Github Rails Installation instructions. learn to read, look that shit up.
