# clean-code-practices

## Priciples taken out from the
https://google.github.io/eng-practices/review/reviewer/standard.html

- ### Maintainability, readability, and understandability of the system
- ### Sharing knowledge is part of improving
- ### Technical facts and data overrule opinions and personal preferences
- ### Style guide is the absolute authority
- ### Aspects of software design are almost never a pure style issue or just a personal preference
- ### Consistent with what is in the current codebase
- ### Come to consensus

## Priciples taken out from the
https://google.github.io/eng-practices/review/reviewer/looking-for.html

- ### Design questions:
    Do the interactions of various pieces of code in the CL make sense?  
    Does this change belong in your codebase, or in a library?  
    Does it integrate well with the rest of your system?  
    Is now a good time to add this functionality?  
- ### Functionality:
    Does this CL do what the developer intended?  
    Is what the developer intended good for the users of this code?  
    The “users” are usually both end-users and developers  
    Think about edge cases  
    Look for concurrency problems  
    Try to think like a user, and making sure that there are no bugs that you see just by reading the code  
    Parallel programming that could theoretically cause deadlocks or race conditions  
- ### Complexity
    Is the code more complex than it should be?  
    Are individual lines too complex?  
    Are functions too complex?  
    Are classes too complex?  
    “Too complex” usually means “can’t be understood quickly by code readers.”  
    It can also mean “developers are likely to introduce bugs when they try to call or modify this code.”  
    Avoid over-engineering  
- ### Tests
   Tests correct, sensible, and useful  
   Tests do not test themselves, and we rarely write tests for our tests—a human must ensure that tests are valid  
   Tests should fail when the code is broken  
   If the code changes beneath them, will they start producing false positives?  
   Does each test make simple and useful assertions?  
   Are the tests separated appropriately between different test methods?
   Don’t accept complexity in tests just because they aren’t part of the main binary  
- ### Naming
   Good name is long enough to fully communicate what the item is or does, without being so long that it becomes hard to read  
- ### Comments
   Clear comments in understandable English  
   Are all of the comments actually necessary?  
   If the code isn’t clear enough to explain itself, then the code should be made simpler  
   Comments are for information that the code itself can’t possibly contain, like the reasoning behind a decision  
- ### Style
   Use the style guide  
- ### Documentation
   On changes how users build, test, interact with, or release code, check associated documentation generated reference docs  
   On deletes or deprecates code, consider whether the documentation should also be deleted  
- ### Every Line
   If you can’t understand the code, it’s very likely that other developers won’t either
- ### Good things
    Is this code improving the health of the system or is it making the whole system more complex, less tested, etc.?  
    Don’t accept code that degrade the code health of the system  
    Most systems become complex through many small changes that add up  
    Prevent even small complexities in new changes
    
   
