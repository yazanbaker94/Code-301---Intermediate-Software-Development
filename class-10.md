1.  What is a ‘call’?
The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.


4.  How many ‘calls’ can happen at once?

stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

6.  What does LIFO mean?
LIFO: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.



8.  Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

        function firstFunction(){
          console.log("Hello from firstFunction");
        }

        function secondFunction(){
          firstFunction();
          console.log("The end from secondFunction");
        }

        secondFunction();

10.  What causes a Stack Overflow?

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.



<hr>

1.  What is a ‘refrence error’?
This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

3.  What is a ‘syntax error’?
4.  I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

6.  hat is a ‘range error’?
7.  Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

9.  What is a ‘tyep error’?

Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.


11.  What is a breakpoint?
 You can also add conditional breakpoints by right-clicking a previous set breakpoint, which will make your program stop at that point only if a condition is met, this is awesome for when you want to debug huge cycles for specific values. 


14.  What does the word ‘debugger’ do in your code?

The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.
