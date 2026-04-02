1 -> HTML5-Semantics
->HTML semantics refers to the use of HTML tags that provide meaning to the content within the tags. These tags help search engines to understand the structure and content of a webpage.
->Semantic HTML tags can also used to improve the accessibility and SEO of a website, as well as making it easier for developers to understand the structure of the webpage. It also helps to ensure that the content is properly structured and organized, which can improve the user experience.
->Some common semantic HTML tags are-
1. <header>: This tag is used to define the header of a webpage.which contains the logo,navigation bar and etc.
2. <nav>: This tag is used to define the navigation menu of a webpage.which contains links like home,about,contact etc.
3. <main>: This tag is used to define the main or actual content of a webpage.This tag contains the actual information that the user is looking for.
5. <section>: This tag is used to define a section of content on a topoic.
6. <footer>: This tag is used to define the footer of a webpage. which typically contains copyright information, contact information, and other important links.
7.<article> tag is also a semantic tag.

2 -> CSS3 layouts and responsiveness
->CSS3 provides 2 various layout techniques for creating responsive web designs they are flexbox and grid.
->Flexbox is a one-dimensional layout system that allows you to create flexible and responsive layouts. It is designed to distribute space along a single axis, either horizontally or vertically. Flexbox is ideal for creating simple layouts, such as navigation bars, card layouts, and form layouts.It uses properties like display:flex, flex-direction, justify-content, align-items, and flex-wrap to control the layout of elements.
->Grid is a two-dimensional layout system that allows you to create complex and responsive layouts. It is designed to distribute space along both axes, horizontally and vertically. Grid is ideal for creating more complex layouts, such as magazine-style layouts, dashboard layouts, and multi-column layouts. It uses properties like display:grid, grid-template-columns, grid-template-rows, grid-gap, and grid-area to control the layout of elements.
->Both flexbox and grid are powerful tools for creating responsive web designs but in my point of view flexbox is better suited for simpler layouts while grid is better suited for more complex layouts.
-> And for responsiveness we add some extra code in css like @media queries which allows us to apply different styles to different screen sizes.Here some units are used to achieve responsiveness like %,em,rem,vw,vh etc. By using these units we can make our website responsive and adaptable to different screen sizes and devices.
->Example
@media (max-width: 768px) { // This styles apply when the screen width is 768 pixels or less.
  body {
    background-color: lightblue;
  }
}

3  -> JavaScript ES6 features
->In javascript only var keyword was used to declare a variable but in ES6 we have 2 new keywords let and const which are used to declare variables. The main difference between var,let and const is that var is function-scoped while let and const are block-scoped. This means that variables declared with var are accessible throughout the entire function, while variables declared with let and const are only accessible within the block they are declared in.And also with var we can perform hoisting but with let and const we cannot perform hoisting.
//  Hoisting example with var
console.log(x); // Output: undefined.And the value of x can be accessed before it is declared because of hoisting and it will not give error.
var x = 5;  
->Arrow functions which are also called as fat arrow functions.These functions are also used for callbacks and these functions have shorter syntax than regular functions.These functions do not have their own this keyword and they inherit the this value from the parent.
ex-
// Regular function
function add(a, b) {
  return a + b;
}   
// Arrow function
const add = (a, b) =>{
        a + b;
    }   
->There are also some features like Promises and async/await are used to handle asynchronous operations in JavaScript. Promises are a way to handle asynchronous operations by providing a way to handle success and failure cases.At the frist the promises are in pending state and then it can be resolved or rejected based on the data.And now focus on async/await,async/await are used to handle asynchronous operations in javascript because js is a single-threaded language and it can only execute one task at a time. So when we have to perform some asynchronous operations like fetching data from an API or doing reading writing opeartions with the database we use async/await to handle the opeartions.
ex-
async function fetchData() {
  try {
    const response = await fetch(api url);
    console.log(response);
  } catch (err) {
    console.log("Some error is courrewd",err);
  }
}
//  Here we also used try and catch these are used to handle error.in try block we put the code that may be give an error and in catch block we log the error.
-> Destructuring is also a feature in js that allows you to get values from arrays or properties from objects and assign them to variables.It can be used by both arrays and objects.
ex-
// Destructuring an array   
const arr = [1, 2, 3];
const [a, b, c] = arr; // here a=1, b=2, c=3
// Destructuring an object
const obj = { name: "Amit", age: 20 };
const { name, age } = obj; // here name="Amit", age=20
->  Also an a important feature is `` Template literals which helps us to print values in a string without using any "," operator.
ex-
const name = "Amit";
console.log(`My name is ${name}`); // Output: My name is Amit

4 -> ReactJS
->ReactJS is a JavaScript framework for building user interfaces. It was developed by Meta and is widely used for building web applications.In react we can create reusable components whiuch can be used in different parts of the applications.Like a application contains multiple buttons then we can create a button component and use it in different parts of the application.
->In react we can not direct communicate with DOM so here a virtual DOM is used to communicate with the real DOM.So virtual DOM is a  copy of the real DOM so when we change something in the ui the virtual dom compare with the real dom and update only the changed part in the application so the application not reload the whole page and it will give better performance.
->React also uses a unidirectional data flow which means that data flows in one direction from parent component to child component. This makes it easier to manage the state.But in large applications it can be difficult to manage the state and pass data between components. To solve this problem we can use state management libraries like Redux or Context API.
->React also provides a feature called hooks like useState and useEffect which allows us to manage state and side effects in functional components.
Also a hook called useContext this hook is used to manage the data in the application and it is used to pass data from one component to another without using props drilling.
In react we also perform two way binding to manage the form data.
->And basically i use 4 layers architecture in my react application like-
1.UI layer //  which can also responsible for the design of the application.
2.Hook Layer // which is responsible for managing the api layer and state layer.
3.State Layer // which is responsible for managing the state of the application,here we perform the useContext the hook to manage the state of the application.
4.API Layer // which is responsible taking data from the backend.

5 -> Performance optimization in ReactJS
->There are several ways to optimize the performance of a ReactJS application. Some of the common techniques include:
1. Code splitting: This technique allows you to split your code into smaller chunks, which can be loaded on demand. This can help to reduce the initial load time of your application and improve the overall performance.
2. Lazy loading: This technique allows you to load components or modules only when they are needed. This can help to reduce the initial load time of your application and improve the overall performance.
3.Avoiding unnecessary re-renders: React components re-render when their state or props change. To optimize performance, you can use techniques like memoization or shouldComponentUpdate to prevent unnecessary re-renders.

6 -> Accessibility in web development
->Accessibility in web development refers to the practice of making websites and web applications usable by people with disabilities.
->Some common accessibility features include:
1. Alternative text for images: This allows screen readers to describe the content of images to users who are visually impaired.
2. Keyboard navigation: This allows users to navigate a website using only a keyboard, which is important for users who are unable to use a mouse.

7 -> GIT
->Git is a version control system that allows developers to track changes to their code and collaborate with other developers.
-> Git workflow command are 
1.git init //  by this command we can initialize a git repository in our project.
2.git add . // by this command we can add all the files to the staging area.
3.git commit -m "message" // by this command we can commit the changes to the repository.
4.git remote add origin "you github repo link" // by this command we can add a remote repository to our local repository.
5.git push -u origin main // by this command we can push the changes to the remote repository.
//  And for changing the branch the command is (git branch -M main/master).

8 -> Typescript
->TypeScript is a superset of JavaScript that adds static typing to the language. It allows developers to catch errors at compile time, rather than at runtime, which can help to improve the overall quality of the code.

9 -> Frontend Architecture 
->Frontend architecture refers to the design and structure of the frontend of a web application. It involves organizing the code and components in a way that is maintainable, scalable, and efficient.
-> Basicallu the architecture are helps in collabarative developement because the developers can easily understand the structure of the application and can work on different parts of the application without any confusion. It also helps in improving the performance of the application because the code is organized in a way that is efficient and easy to maintain. And also it helps in improving the user experience because the code is organized in a way that is easy to understand and navigate.
-> I work on 4 layers architecture in my react application i work on features based architecture.In this architecture we organize the code based on the features of the application.For example if we have a e-commerce application then we can organize the code based on the features like product listing,product details,cart,checkout etc.This architecture helps me a lot to improving the maintainability and scalability of the application because the code is organized in a way that is easy to understand and navigate.It also helps in improving the performance of the application because the code is organized in a way that is efficient and easy to maintain.