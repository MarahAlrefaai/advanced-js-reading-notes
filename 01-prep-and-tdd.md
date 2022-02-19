### JavaScript
its singlr threaded programming language (do one thing at time ).
------------------------------------------------------------------------------

### call function 
calling function  inside another function  and then take the result to do operation on it if it exist (LIFO) principle.
In JavaScript, functions are objects.
 we can pass objects to functions as parameters
------------------------------------------------------------------------------

Functions running in parallel with other functions are called asynchronous
A good example is JavaScript setTimeout()
### settimtout(fun,time)
execute the operetion after the time that spicified and then put it in the queue to run it after the stack is empty 
------------------------------------------------------------------------------
### Promise
Multiple callback functions would create callback hell that leads to unmanageable code.
Also it is not easy for any user to handle multiple callbacks at the same time.
so the solution is using (Promise)
Promise.then then(function () {
      Success
    }).
    catch(function () {
       error
    });
------------------------------------------------------------------------------

### Async/Await
 keyword async before a function makes the function return a promise.
 keyword await before a function makes the function wait for a promise.
------------------------------------------------------------------------------
### Test-Driven Development
 Testing is the process of ensuring a program receives the correct input and generates the correct output and intended side-effects. 
  types:
  1-Manual Testing
  2-Automated Testing

  Test-driven development is the act of first deciding what you want your program to do (the specifications), formulating a failing test, then writing the code to make that test pass.



