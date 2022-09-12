# Vaihe 1 - #Q1

## Bug ticket #6341

Hello from the QA team,

We noticed that there's no input sanitazion in the check person method. Someone was trying to be funny, and made a successful payment named as "Michael
Looooooo&lt;truncated&gt;oooooooooooooong". 

1) unskip the long name test in `payment-01.test.js`
2) fix the code. Let's only allow max 40 character names
3) rerun the tests and check that it passes

ーAndrew

## Feature request #6342

According to previous discussion, we are dropping support for Amex cards. I added a skipped test to `payment-01.test.js`. Please unskip the test and fix the code accordingly.

1) unskip the Amex card test
2) fix the code
3) rerun the tests and check that it passes

## Bug ticket #6343

Someone is trying to insert floating numbers (eg. 1.33334) into our payment api, but we only support integers (eg. 1, 5, 100). I added a skipped test to `payment-01.test.js`. Could you:

1) unskip the invalid payment object test
2) fix the code. Maybe this StackOverflow link helps? https://stackoverflow.com/questions/3885817/how-do-i-check-that-a-number-is-float-or-integer
3) rerun the tests and check that it passes

ーAndrew

[Step 0](./ASSESSMENT.md) ・
[📖 Step 1](./ASSESSMENT1.md) ・
[Step 2](./ASSESSMENT2.md) ・
[Step 3](./ASSESSMENT3.md)