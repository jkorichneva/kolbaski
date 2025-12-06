# Using the yieldToMain utility

If we have long microtasks but want to schedule them in a way that they are not interfering with the user input we
can use yieldToMain function. Before applying yieldToMain we see that first the microtasks are being executed and
after the user input is being handled.

![without Yield]('./withoutYield.png)

After applying we see that microtasks are split and allow to handle user input.

![with yield]('./withYield.png)
