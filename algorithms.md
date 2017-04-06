# Algorithms

## Pseudo Code

Pseudo code is the process of taking a larger solution and breaking it down into the programmable steps without actually writing any code.

1. Think about the larger solution as a whole, but as a series of steps that you would write out for a petulant child to follow
1. Write out the solution in plain English, breaking it down into as many tiny steps as possible.  Remember, this child doesn't want to do the task.  If there's any ambiguity, you're sunk
1. Create a flow chart
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
