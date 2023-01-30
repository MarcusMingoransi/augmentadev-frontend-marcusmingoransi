# augmentadev-frontend-marcusmingoransi

## JavaScript Developer - Technical questions

### Question 1:
**What is a closure?**

**Answer:**
It is a programming language concept that allows a child function to access variables from its parent function. The parent function will return a reference to the child function and every time we call a child function the variable and the parent function will change its value instead of being reset.

<img width="213" alt="image" src="https://user-images.githubusercontent.com/8353673/215521941-1e9f28f7-15b7-495b-ab8e-8819eb7137f4.png">


### Question 2:
**a) In a garbage-collected language like JavaScript, how are memory leaks possible?**

**Answer:**
This occurs when a part of the memory should be released but is not. A good example is when we forget to stop an interval that we created. Other examples are: referencing a non-existent variable in a global scope that will create a new object or variable, and also forgotten global variables.

**b)  Can you describe the low-level mechanics of a memory leak?**

**Answer:**
Javascript is smart enough to allocate memory when we create an object or a variable and clear it when it is no longer needed, but some flaws in the logic of the code can cause this object or variable not to be cleared as it should be, which causes loss of performance and unexpected errors.


### Question 3:

**a)	What is dead code?**

**Answer:**
It is a piece of code that is no longer used or repeated code. It can be a variable, an object, a parameter or a class.


**b)  How is dead code elimination done in JavaScript?)**

**Answer:**
There are some tools that help us with this. You can use eslint which is a library that checks if a variable, object or function is being used or not and if not, return some warnings helping the programmer to remove dead code. Another option is to use the "webpack-deadcode-plugin", and add it to the application's webpack so it doesn't compile files that are not being used, avoiding a larger size of the final build. Another option if you use Typescript is to use the "ts-prune" library that allows us to find a list of unused exports every time we run the command from it that we defined in the package.json.

**c)  What would be the challenges in implementing a dead code elimination tool for JavaScript, as opposed to one used in a statically-typed language such as C++ or Java?

**Answer:**
Since JavaScript is dynamically typed, this makes it harder to determine the types of variables, objects, functions, and so on. Event handling functions of HTML elements also make it harder to identify if it is dead code. Also, DOM handling events.

### Question 4:

**JavaScript performance has improved significantly since it was first released in 1995. What are the key changes in the history of JavaScript that have enabled this?**

**Answer:**
There have been some significant changes such as the release of Google v8, which allows for a much faster runtime. The adoption of JIT and AOT to improve application compilation. Lazy loading that allows loading some code only when the developer really needs it to be executed, this makes the application initially lighter and consequently increases the web page loading speed. The adoption of ECMAscript brought new features and syntax changes to improve performance.


### Question 5:

**Is it possible that new future language features in JavaScript will be able to improve the performance of applications? Or, would you expect new language features, in general, to have either zero or negative effect on performance? Why or why not?**

**Answer:**
Any new feature that is implemented can have good or bad results, if it is bad, it can cause more complexity or worse memory management or worse processing or even a change in the behavior of some part of the code that can lead to a bug, but if it is good it can make the application lighter, faster to run, more readable, new native functionality that before was done through third party libraries, which helps to reduce the size of the application build. In short, an update that adds benefits is very welcome to further enrich JavaScript.

