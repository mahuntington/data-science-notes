# Algorithms

## Lesson Objectives

1. Define what an algorithm is
1. Describe situations in which we use algorithms in data science
1. Describe the process for creating an algorithm
1. Create some algorithms of your own

## Define what an algorithm is

An algorithm is just a series of steps to be taken.  It's what computers use to solve a problem

## Describe situations in which we use algorithms in data science

1. Grab information from the internet and present results
    - What's happening in social media?
1. Given a set of data files, produce charts
    - Provide analysis of a company's performance
1. Help a website provide meaningful data to users
    - What posts are "trending"?
1. Machine Learning
    - purpose
        - representation
            - extract data from data
        - generalization
            - make predictions from data
    - forms
        - supervised
            - Usually requires data verified by humans
            - Using existing data
                - extract meaning from it
                - make predictions with it
            - Example 1
                - Feed a computer scans of brains with cancer
                - Have The computer make predictions about whether or not new images of brains show cancer
            - Example 2
                - Given actions of a driver, teach a computer how to drive
            - Example 3
                - Suppose you want to predict whether someone will make make a purchase the week after they visit your site.
                - You have a set of data on previous customers, including age, interests, previous purchases, time of visit, etc.  
                - You know whether previous customers made a purchase within a week of their last visit.  
                - So, the problem is combining all the existing data into a model that can predict whether a new person will make purchase within a week.
                - You can then take action and send a reminder or offer a discount.
                - Amazon, Netflix, and others do this based on the history of their existing customers.
        - unsupervised
            - the computer will look at data and create relationships itself so it can
                - extract meaning from it
                - make predictions with it
            - Example
                - Suppose you want to understand your customer base so that you can produce appropriate segments that you can target with your next marketing campaign.
                - You have a set of data about your customers, including age, location, previous purchases, time of visit, etc.
                - But what characteristics should you use?
                - Based on these attributes the program will find similarities and differences that provide groupings (segments) of customers.
                    - it will figure out people like
                        - the hedge fund manager's playboy son
                        - the single mother
                        - the angsty tween
                - You can then take action and make an offer or recommend a product specifically to these segments.

## Describe the process for creating an algorithm

### The process

To create an algorithm for a computer program, there are a few steps to follow:

1. Think about the larger solution as a whole, but as a series of steps that you would write out for a petulant child to follow
1. Write out the solution in plain English, breaking it down into as many tiny steps as possible.  Remember, this child doesn't want to do the task.  If there's any ambiguity, you're sunk
1. Create a flow chart (decision tree)
    ![musical flow chart](http://i.imgur.com/J1iNj.jpg)
1. Write Pseudo code for the algorithm (explained below)
1. Write computer code to solve the issue

### What is Pseudo Code?

Pseudo code is the process of taking a larger solution and breaking it down into the programmable steps without actually writing any code.

1. Try to separate each phrase/independent clause onto a different line
1. Identify the following:
    - Assertions
        - comments, probably
    - Conditionals
        - A question is asked.  This tells us a conditional is coming
        - Looks for words like "if, unless, otherwise"
        - Think of all the possible outcomes of the situation
            - Each outcome represents an `if`, `else if`, or `else` statement
    - Loops
        - Something is done multiple times
        - Look for words like "while, as long as, until"
        - Think of the child asking "am I done yet?"
            - Better to tell them "keep eating string beans until there are no more string beans" than to tell them to each individual string bean
    - Functions
        - We've oversimplified a step which could be broken out into multiple steps.
1. Identify data types
    - whenever you have a conditional, loop, or something you're keeping track of, identify its type
        - text (strings)
        - numbers (ints/floats)
        - true/false values (booleans)
        - collections of stuff (arrays)
1. (Optional) Try to convert each line into something that resembles code

Example:

```
Peeling an orange: First, do we have an orange?  If not, I'm going to take one out of the fridge.  We now have the orange.  Then I'm going to see if it has already been peeled.  If it is peeled, I'm going to eat it.  If it isn't peeled, I'm going to remove a chunk of the rind.  At this point, I'm going to see if it's peeled.  If it isn't I'm going to remove another chunk of the rind.  I'll keep doing this until the orange is peeled.

Do we have an orange? - conditional coming up
    We do not have the orange: - conditional (boolean test: does orange exist)
        Take out the orange - function
We now have the orange - comment
Is it peeled? - conditional coming up
    If it is peeled - conditional, situation 1 (number test: number of pieces of rind left === 0)
        You're done!  Eat it! - function
    If it is not peeled  - conditional, situation 2 (number test: number of pieces of rind left > 0)
        As long as it is not peeled - loop (number test: while(number of rind pieces > 0))
            Remove a chunk of rind - function
        The orange is now peeled - comment
        You're done!  Eat it! - function
```

## Create some algorithms of your own

Do the following in groups:

1. Write pseudo to to make a peanut butter and jelly sandwich
1. Given a bunch of votes on a post, create a "Recently Popular" algorithm
    - like Reddit
