# Example with fetching via Promise.all()

## Pictures

## What is happening:
We put two promises into Promise.all() and after they are resolved we execute some code via .then().
If we have a longer blocking task in the event loop the callback for the Promise.all() is being put into the call stack after the main thread is empty.
As expected, it is executed before setTimeout callback as it is a microtask.
