Do at least ONE of the following tasks: refactor is mandatory. Write tests is optional, will be good bonus to see it. 
Please do not invest more than 2-4 hours on this.
Upload your results to a Github repo, for easier sharing and reviewing.

Thank you and good luck!



Code to refactor
=================
1) app/Http/Controllers/BookingController.php
2) app/Repository/BookingRepository.php

Code to write tests (optional)
=====================
3) App/Helpers/TeHelper.php method willExpireAt
4) App/Repository/UserRepository.php, method createOrUpdate


----------------------------

What I expect in your repo:

X. A readme with:   Your thoughts about the code. What makes it amazing code. Or what makes it ok code. Or what makes it terrible code. How would you have done it. Thoughts on formatting, structure, logic.. The more details that you can provide about the code (what's terrible about it or/and what is good about it) the easier for us to assess your coding style, mentality etc

=+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+=
=+=+==+=+==+=+==+=+== Reason, Changes And Thoughts ==+=+==+=+==+=+==+=+==+=
=+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+==+=+=

I have changed some of the code in controller but not much in the repository. The changes I made are due to these reasons

1. Variable scope is important because if variables are declared but never used, its considered a bad practice.
1.1. Variables can confuse the new reader/developer if not properly used.
1.2. If a variable is used only once and there is no other point in cycle that variable is modified then it is best to avoid using variable.
1.3. Unused variables should be commented or removed from the code.

2. Using assignment in control flows (If, If-else) is not very good move (imo).
2.1. This type of code can sometimes make it hard for testing or reviewing.
2.2. Control flows should always have a default/non-blocking statements to prevent system blocking. (Else phrase or default values)

3. Non-usage of loop index is not a bad practice but if an external variable is used then it is a no-no situation.
3.1. Loop's own index should be preferred where we need to keep track (In most cases loop index is same as of Language recommended).
3.2. Each loop has its own merits and demerits, keep them in mind when deciding about the usage.

About the changes I made:
A. In Booking Controller, I made many changes.
A.1. Removed assignments in control flow statements.
A.2. Removed variables that are not required for proper functioning.
A.3. Using language/platform helper functions to simplify conditions and code readability.

B. In Repository, I made vary few changes.
B.1. Commented unused variables.
B.2. Simplified some control flow statements.

My thoughts about the code:
I observed that controller and repository were written by different developers (This is only an observation it can be wrong).
Code was well written and had very limited scope of changes. Optimization of the code was kept in mind while writing.
Only some personal level practices were to be seen on many places.
Code was properly commented on some places but on some places comments were nowhere to be seen. I also sometimes miss proper commenting for documentation.
But it is a good practice to keep the code simple and descriptive (for any new member to understand).
Overall code was good and readable and understandable.
In some places like in repository, some functions/methods were too large so some separation is required (I could not do it without proper context).
