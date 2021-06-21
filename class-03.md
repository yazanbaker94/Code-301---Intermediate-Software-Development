# React Docs - lists and keys


1. What does .map() return?
  map() function returns a map object(which is an iterator) of the results after applying the given function to each item of a given iterable (list, tuple etc.
3. If I want to loop through an array and display each value in JSX, how do I do that in React?
  The map() method is the most commonly used function to iterate over an array of data in JSX. You can attach the map() method to the array and pass a callback function that gets called for each iteration. When rendering the User component, pass a unique value to the key prop
  
5. Each list item needs a unique ____.
 string 
7. What is the purpose of a key?
Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:


1. What is the spread operator?

The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.


3. List 4 things that the spread operator can do.

Copying an array
Concatenating or combining arrays
Using Math functions
Using an array as arguments


5. Give an example of using the spread operator to combine two arrays.
        const myArray = [`🤪`,`🐻`,`🎌`]
        const yourArray = [`🙂`,`🤗`,`🤩`]
        const ourArray = [...myArray,...yourArray]
        console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩
        
        
7. Give an example of using the spread operator to add a new item to an array.

        const fewFruit = ['🍏','🍊','🍌']
        const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
        console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]


9. Give an example of using the spread operator to combine two objects into one.

        const objectOne = {hello: "🤪"}
        const objectTwo = {world: "🐻"}
        const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
        console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
        const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
        objectFour.laugh() // 😂😂😂😂😂



1.  In the video, what is the first step that the developer does to pass functions between components?
uses the state and uses the map function.
2.  In your own words, what does the increment function do?
the increment function updates the count based on what name the is passed into the arguement - name
3.  How can you pass a method from a parent component into a child component?
this.setState
5.  How does the child component invoke a method that was passed to it from a parent component?
pass down functionality to children in props
