 
 # Read 3
## React Docs - lists and keys.
 1-What does .map() return? array 

  2-If I want to loop through an array and display each value in JSX, how do I do that in React? include them in JSX using curly braces {}.

  3-Each list item needs a unique a key.

  4-What is the purpose of a key?is a special string attribute you need to include when creating lists of elements.

  ## The Spread Operator
1-What is the spread operator?

 in  JavaScript, spread syntax refers to the use of an ellipsis of three dots (âĶ) to expand an iterable object into the list of arguments.

    1-Copying an array.

    2-Concatenating or combining arrays

    3-Using Math functions.

    4-Using an array as arguments.

    5-Adding an item to a list.

    6-Adding to state in React.

    7-Combining objects.

     8-Converting NodeList to an array.

3-Give an example of using the spread operator to combine two arrays.


const myArray = [`ðĪŠ`,`ðŧ`,`ð`]
const yourArray = [`ð`,`ðĪ`,`ðĪĐ`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // ðĪŠ ðŧ ð ð ðĪ ðĪĐ.


Give an example of using the spread operator to add a new item to an array.

const fewFruit = ['ð','ð','ð']
const fewMoreFruit = ['ð', 'ð', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "ð", "ð", "ð", "ð", "ð" ]

Give an example of using the spread operator to combine two objects into one.
const objectOne = {hello: "ðĪŠ"}
const objectTwo = {world: "ðŧ"}
const objectThree = {...objectOne, ...objectTwo, laugh: "ð"}
console.log(objectThree) // Object { hello: "ðĪŠ", world: "ðŧ", laugh: "ð" }





In the video, what is the first step that the developer does to pass functions between components?

Create the function where he want to change the state inside.
In your own words, what does the increment function do?

It increment the count inside the state by one.
How can you pass a method from a parent component into a child component?

Using props.
How does the child component invoke a method that was passed to it from a parent component?

Create another function inside the child component.
Things I want to know more about