1.    What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 


2.  What is a pure function and how do we know if something is a pure function?

It returns the same result if given the same arguments (it is also referred as deterministic)
It does not cause any observable side effects


3.  What are the benefits of a pure function?
It returns the same result if given the same arguments

4.  What is immutability?
Unchanging over time or unable to be changed.


5.  What is Referential transparency?

pure functions + immutable data = referential transparency


<hr>


1.  What is a module?
The Module pattern is used to mimic the concept of classes (since JavaScript doesn't natively support classes) so that we can store both public and private methods and variables inside a single object


2.  What does the word ‘require’ do?
The require() method is used to load and cache JavaScript modules. So, if you want to load a local, relative JavaScript module into a Node. js application, you can simply use the require() method.

3.  How do we bring another module into the file the we are working in?
The static import statement is used to import read only live bindings which are exported by another module.

4.  What do we have to do to make a module available?

The first thing you do to get access to module features is export them. This is done using the export statement. You can export functions, var , let , const , and — as we'll see later — classes. They need to be top-level items; you can't use export inside a function, for example
