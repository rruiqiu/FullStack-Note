# HTML

HTML = HyperText Markup Language

Codepen is a strong online learning IDE;

heading element goes from h1 to h6;('<h1> </h1>')

h1= largest, h6=smallest;

boilerplate, a template for the html

```html
<br> <!-- used to create an empty line -->

<hr> <!-- making a horzintal line -->

<!--"This is where"you can put comment in HTML  -->
```

 Some things to learn

ordered list, <ls>

```html
  <ol type="i"> <!-- type to identify the ordered list symbol -->
    <li>Microprocess Project</li>
    <li>Leetcode cookbook in cpp</li>
    <li>McMaster Recycling Plant Project</li>
    <li>Personal Website</li>
  </ol>
```

unordered list <ul>

```html
  <ul>
    <li>HTML/CSS/Javascript</li>
    <li>C/C++</li>
    <li>Python</li>
    <li>SQL/Mysql/Golang/Django</li>
  </ul>
```

table <table>  <tr>- table row, <td> table data

```html
  <table cellspacing=10>
    <thead>
      <tr>
        <th>Date</th>
        <th>Work</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>2010-2013</td>
        <td>Lead Developer</td>
      </tr>
      <tr>
        <td>2019</td>
        <td>INssda</td>
      </tr>
    </tbody>
```

hyperlink <a href = ""><a/>

```html
<a href="https://github.com/richardddddddd"><img src="images/github-logo.png" alt="github"
            style="max-width: 3%;"></a>
```

//span can be used when not want to start a new line.

span cant change width



# CSS

CSS = Cascading Style Sheets

```
change the body background of css
```

Grammar:  selector{property:value;}

id can only use in one place

class can be used in different places

Class can have more than one attributes in one element, id can only have one 



Solving the problem if the icon isnt shown up in the browser - add [?v=2]



Div - used to structure: stands for a content division element



Display; inline and block, inline is for the content without occupying a line vice versa for the block element.

Inline-block; useful to change the width also without occupying the line

Dispaly none; remove elements from the website,

Visiblitity:hidden. used to hide the elements from the web but still occupying the original position



## Absolute Position and Relative Postion, Float

Relative Postion: Change the postion by calling the top, right, left, bottom with px to its corresponding original position

Absolute Position: Absolute position relative to its parent div

Fixed Position: Scroll the web page won't influence the top fixed position element

Float: float used to float img on the right or left, used to wrap text around imp

## Font size

font size(used for pecertange change): 16px = 100%,  90px = 90px/16 =562.5%

em: = M, the width of 1em = 1times the capital size of M, 1em =16px

16px=100%=1em. to obatain dynamically, 90px =5.625em

em can be inherited(added) from other styles both em and % will have that but px will not.



rem ignore other parents setting same function as px



## Z-index



## Media-Query Breakpoint



## Combine selectors in css

Able to select Id by defining another class

#heading .container-fluid

Combine selectors in css

## Hierarchical Selectors

#heading .container-fluid

spacing is crucial

Read the hierchi from right to left

right is a child, left is parent

only work when child is inside the parent



## Multiple Selectors

Selector1, selector2{

}



# Bootstrap

Wireframing always comes first, https://balsamiq.cloud/ a good toop to learn

## Grid

12quarters(parts) of the screen:

## A Note About CSS Link Order

A note about CSS link Order that it will process from top to bottom, that means if we want to add our own css styles, we need to put it after the bootstrap link.

## Note about using newest google font

the font with the weight adjusting can be setting by imorting the range, the font without range need to speicfy a typical font weight as the same setting shown in the google font also need to import in the html head link file

## Carousel/Slide show

Use card-group instead of card-deck for horizontal display

# Javascript

alert("Hello");

alert("World");

output Hello

## Datatype

```javascript
String - "Hello";

Numbers;

Boolean - true and false

typeof() - to identify the data type of variable


```

## Get input

prompt("what is your name");

//allow ueser to input something



## Var

Var myName = "Angela";

## Naming convention

give your variables meaningful name

Star the first letter with lowercase then become the upper case

## Length

var name.length;

## Slice

slice(x,y);

slice the range from x to y;

the string range index start with 0;

## Uppercase/Lowercase

<variable>.toUpperCase()

change the string of variable to uppercase

vice versa for lowercase

## Modulo

Remainder

6%4 = 2;

12 % 8 =4;

Notice:

3%10 = 3;

## Notice incrementing order

var x= 3;
var y=x++;

Output; y =3;

In your assignment `y = x++;` the value of **y** is first assigned to **x** and then the variable **x** gets incremented by 1. By performing this operation **y** becomes 3 and x is 4. Then after running y +=1 computer will calculate 3+1 = 4; So to expecting 4 it should be equal to `y = ++x`;

## Functions

Syntax:

`function variable( ){ command	}`

it can also give an output by using the return by assigining a variable





## console.log( )

log all those commands into console command space;

alert - user can see

console.log( ) - meant for the developer to see

## Random number generator

//pseudo number generator

var n = Math.random();

between 0 and 0.99999 - 16decimal places

to get beyond 1; mulitply by a large number

we can mulitply an assigned number which identifies the range between 0 and smaller than this assigned number

```javascript
//Example: generate number from 1 to 6;

var n = Math.random();

Math.floor(n* 6)+1; //floor round down number to the nearest integer

//Output 1-6; 


```

## Control Statements: If-Else

if equal to use three equal signs: ===;

if, else if, else;



```
=== is equal to(also check to see the datatype)

!== is not equal to

> is greater than

< is lesser than

>= is greater or equal to

<= is less or euqal to

== is equal to (not care about data type)
```

## Combining Comprartors

&& AND

|| OR

! NOT

## Arrays

Var eggs = [ ]

Start with the position zero

can call the inner element by specifying the index number

var.includes( );

findout if an arry include a particular element, will return a boolean(true of false)

var.push(element); // push element to the back at the back

var.pop; //pop up the last element of the array

## While loops/For loops

for(i=0;i<2;i++){

​	DO SOMETHING

}

# DOM

Document Object Model - DOM

```javascript

document.getElementByTagName
document.getElementsByClassName
document.getElementByID

.innerHTML //can change the text of HTML elements

document.querySelector("id,class,tag") //select the input type of the website
//also will return the first class with the same name if appeared in the html

document.querySelectorAll() //will return a Nodelist that can be called the index of elemnt like arry
document.querySelectorAll()[num]
```



Able to add a class list, remove list or toggle list;

```
document.querySelector("").classlist.add("from style class list");

document.querySelector("a").getAttribute("href");
document.querySelector("a").setAttribute("href", "link");
```



## addEventListener

```javascript
document.querySelector("button").addEventListener("click", handleClick)
function handleClick () {
  alert("I got clicked!")
}
//passing a function when the event is being triggered
//will directly call the function if the parameter is written as handleClick() inside the addeventlistener
```



## Select all Elements in Dom

```javascript
for (var i = 0; i < document.querySelectorAll(".drum").length; i++) {
  document.querySelectorAll(".drum")[i].addEventListener("click", handleClick)
  function handleClick () {
    alert("I got clicked!")
  }
}
```

## Higher Order functions

functions that can be called in higher order functions

which means functions can also be passed as an arguement 

## Play Sounds in Javascript

## this

this- can get the object of the current using element

## Object

Like object oriented 

```javascript
var housekeeper= {
    age: 16,
    country: "china",
    clean: ["bathroom", "lobby", "basement"]
        
    
}

housekeeper.clean

//Constructor function
var nnn = new bellboy("timmy",19,true,["1","2","3"])
```

Construction Function and use

```javascript
function Housekeeper(yearsofExperience, name, cleaningarea){
    this.yearsofExperience = yearsofExperience;
    this.name = name;
    this.cleaningarea = cleaningarea;
}

var Housekeeper1 = new Housekeeper(9, "zeno", ["lobby","bathroom"])
console.log(Housekeeper1)
console.log(Housekeeper1.name)
```

## Object.Method

directly add a function inside the constructor function

```javascript
function Housekeeper(yearsofExperience, name, cleaningarea){
    this.yearsofExperience = yearsofExperience;
    this.name = name;
    this.cleaningarea = cleaningarea;
    this.clean = function(){
    	alert("Cleaning in progress..")
    }
}

var Housekeeper1 = new Housekeeper(9, "zeno", ["lobby","bathroom"])

Housekeeper1.clean();
```



## Switch

Similar to cpp

```
switch(expression){
 case expression:
 
 break;
 default;
}
```

## KeyBoard Interruption

```javascript
document.addEventListener("keydown", function (event) {

  makeSound(event.key) // to findout the specific key and passing the key as a parameter to makeSound

})
```

## Callingback Function

passing a callback function inside the addeventlistener and it can return the information from the event trigger

# jQuery(framework)

A library to make your life easier

```javascript
document.querselector("h1") = jQuery("h1") = $("h1")

$ = document.querselectorall("button")//. Also

$("h1").css("color", "green")//, is setting the value

$("h1").css("font-size")//, is by getting the property

$("h1").addClass("<a defined class list from stylesheet>") by adding more class simply put an empty space

$("h1").removeClass("<a defined class list from stylesheet>")

$("h1").hasClass("<a defined class list from stylesheet>") //retrun true of false if it contains the specific class

$("h1").text("text content that will replace the h1") //retrun true of false if it contains the specific class

$("button").html("<em>Hello</em>") //inner Html method

$("img").attr("src"); //can get the source link from console.log

$("a").attr("href"," new link") //setting the new link for the href.


```



## Adding Eventlistener 

```javascript
$("h1").click(function(){
	$("h1").css("color","purple")
})  //Event listener for h1 click with the specific funciton

$("input").keypress(function(event){
  console.log(event.key);
}) //able to get the input key from the input table

$("document") //by selecting the entire website which use 


```

## Method On

event reference - https://developer.mozilla.org/en-US/docs/Web/Events#event_listing

```javascript
$("h1").on("mouseover",function(){
 $("h1").css("color","purple")
}) //simple eventlistener by using on and giving an attribute
```

## Adding and Removing Elements

```javascript
$("h1").before("<button>New</button>");//adding a new element before the h1 element
$("h1").after("<button>New</button>");//adding a new element before the h1 element
$("h1").prepend("<button>New</button>");//adding a new element after the h1 content opeing tag
$("h1").apeend("<button>New</button>");//adding a new element before the h1 ending h1 closing tag

$("button").remove(); //remove all buttons from document
```

## Websites Animations 

jQuery effect

```javascript
$("h1").hide() //hide elements
$("h1").show() //show elements
$("h1").toggle() //hide or show elements

$("h1").fadeOut() //hiding a reduce disappera animation
$("h1").fadeIn() //
$("h1").fadeToggle() //

$("h1").slideDown() //slide animation
$("h1").slideup() //
$("h1").slideToggle() //

$("h1").animate({opacity: 0.5});  //change the opacity, cant change color 

$("h1").slideDown().slideUp().animate({opacity:0.5}) //chain all the animation in order
```

## Playing Sound

```js
var audio = new Audio("sounds/tom-1.mp3") // src come from
//also notice that it can be used the + to break the src from link
audio.play()
```

# Unix Command Line

## Command Line Tool(Udemy)

- `ls` list all files under the user directory

- `cd` - Change directory, change to the specific directory with the given name, can put enough letters to let the computer know which directory to specify

- `cd~` go back to the root directory

- `↑` `↓` arrow key 

- `cd..` move back one directory, `cd../..` move back two directories

- `option + command` can select the specific location with the mouse clicking

- `ctrl+A` go to the beginning of the command

- `ctrl+E` go to the end of the command

- `control+U` clear the entire command line

- `mkdir` making a new directory

- `touch` create a new file, with creating and adding the extension file

- `open` to open a file

- `open -a Atom Text2.text` open a file with specific application

- ` rm` remove file with given name

- `rm *` remall all files inside the current directory, not folders

- `pwd` print working directory - print the current folder path

- `rm -r directory/` remove a folder/directory all inside folders

  

  Learning enough command lines to be dangerous: https://www.learnenough.com/command-line-tutorial









## Command Line Tool(Codecademy)

- `pwd` outputs the name of the current working directory.
- `ls` lists all files and directories in the working directory.
- `cd` switches you into the directory you specify.
- `mkdir` creates a new directory in the working directory.
- `touch` creates a new file inside the working directory.

- `clear` clears the terminal
- tab autocompletes the name of a file or directory
- ↑ and ↓ allow you to cycle through previous commands
- cd .. (move back one directory), cd ../.. (move back two directories)
- echo "Hello Command Line" >> hello_cli.txt (to create a new file named **hello_cli.txt** and add `Hello Command Line` to that file.)
- `cat hello_cli.txt` to print the contents of the **hello_cli.txt** file to the terminal.

The up and down arrows (↑ and ↓) can be used to cycle through your previous commands. ↑ will take you up through your most recent commands, and ↓ will take you back through to the most recent one.

"tab" can be used to autocomplete your command. When you are typing the name of an existing file or directory, you can use tab to finish the rest of the name.//可以为变量名后缀自动配置



A filesystem organizes a computer's files and directories into a tree structure.



Mac osX, open an empty space.

Error used to occur: string not in pwd: spring 

solving method: (cd spring\ 2021\ classes # This is escaping the spaces)

or (cd "spring 2021 classes" # This is using quotes to inclose)				

​		

Bash = Bourne Again Shell



# Backend Web Development

Full Stack = Front-End + Back-End

Server

Database

Application



Client-Side

Server

Database 

# Node.js

```js
node.index.js //using node to run the index.js on computer
```

- `.exit` to exit node.js in command line tool
- `clear` claer the previous commands
- `const` creat a constant variable that cannot be changed
- `const fs = require("fs")` . Filesystem
- `fs.copyFileSync("file1.txt", "file2.txt")` copy file from file1 to file2, if file2 doesn't exist, create a new file

```js
const express = require("express")

const app = express()

app.get("/", function (req, res) {
  res.send("Server is up and running")
})



app.listen(3000, function () {
  console.log("Server is running on port 3000.")
})
```



## NPM

NPM - Node Package Manager

`npm install <statement>` can find online to search cool npm packages by installing using the command and using their method by following the description 

## Express.js(framework)

allow u to write less repetive code

Create the first server

`npm require express` require the express



```js
const express = require('express')
const app = express()
app.listen(3000, function () {
  console.log("Server started on port 3000")
})

app.get("/", function (req, res) {
  res.send("hello")
  // console.log(request)
})
```

```js
app.get("/", function (request, response) {
  response.send("hello") //also ablt to add html element
  // console.log(request) //get the request from nodejs
})

const express = require('express')
const app = express()


app.get("/", function (req, res) {
  res.send("hello")
  // console.log(request)
})

app.get("/contact", function (req, res) {
  res.send("Contact me at 171197868")
  // console.log(request)
})

app.listen(3000, function () {
  console.log("Server started on port 3000")
})
```

In command line, `node server.js`

`sudo npm install -g nodemon`

`npm i pstree.remy@1.1.0 -D` 

## Simple Calculator

Before we start creating our Calculator website, we'll need to set up a new project. Follow the steps below using your Hyper Terminal to complete this challenge:

- Make a new folder called Calculator on your Desktop
- Change Directory to this new folder
- Inside the Calculator folder, create a new file called **calculator.js**
- Set up a new NPM package
- Open the project folder in Atom 
- Using NPM install the **express** module
- Require express in your calculator.js
- Setup express
- Create a root route get method with app.get()
- Send the words **Hello World** from the root route as the response
- Spin up our server on port **3000** with app.listen
- Run server with **nodemon**



`res.sendFile("index.html")`

`  res.sendFile(__dirname+"/index.html")` _dirname allows to get a constant of the current file

`nodemon calculator.js `



## Body parser

`npm install bodyparser`

```js
const express = require('express')
const bodyParser = require("body-parser")

const app = express()

app.use(bodyParser.urlencoded({ extended: true })) //the code u want to use to get html element 


app.get("/", function (req, res) {
  res.sendFile(__dirname + "/index.html")
  // console.log(request)
})

app.post("/", function (req, res) {  //get the post from the html file
  console.log(req.body)

  var num1 = Number(req.body.num1)   //equal to the name of the input type text
  var num2 = Number(req.body.num2)
  var result = num1 + num2

  res.send("Thanks for typing that, the reuslt of the calculation is" + result)
})

app.listen(3000, function () {
  console.log("Server started on port 3000")
})
```

# APIs

Application Programming Interfaces

An API is a set of commands, functions, protocols, and objects that programmers can use to create software or interact with an external system - Your server request someone's else server

Paramters , Path of the API 

## JSON

JavaScript Object Notation, 

```js

app.get("/", function (req, res) {
  const url = "https://api.openweathermap.org/data/2.5/weather?q=Hamilton,Canada&appid=2c3234ea456e8bc6b29835578f4c1d72&units=metric"
  https.get(url, function (response) { // connenct to the url
    console.log(response.statusCode)

    response.on("data", function (data) {
      const weatherData = JSON.parse(data) //JSON.parse convert the data from hexadecimal to actual data format
      console.log(weatherData)
    })
  })


  res.send("Server is up and running")
})
```

`JSON.stringify(object)` remove all space but keep all syntax

`      const temp = weatherData.main.temp` `.` Used to navigate the objective data

`res.write` can write many times

`res.send` can only have one in app.get for each function

## Weather project

```js
const express = require("express")
const https = require("https")
const bodyParser = require("body-parser")
//const { send } = require("process")

const app = express()

app.use(bodyParser.urlencoded({ extended: true }))

app.get("/", function (req, res) {
  res.sendFile(__dirname + "/index.html")
  //res.send("Server is up and running")
})

app.post("/", function (req, res) {
  const query = req.body.cityName
  const apiKey = "2c3234ea456e8bc6b29835578f4c1d72"
  const unit = "metric"
  const url = "https://api.openweathermap.org/data/2.5/weather?q=" + query + "&appid=" + apiKey + "&units=" + unit
  https.get(url, function (response) {
    console.log(response.statusCode)

    response.on("data", function (data) {
      const weatherData = JSON.parse(data)
      const temp = weatherData.main.temp
      const description = weatherData.weather[0].description
      const icon = weatherData.weather[0].icon
      const imageURL = "http://openweathermap.org/img/wn/" + icon + "@2x.png"

      console.log(temp, description)
      //console.log(weatherData)
      res.write("<p>The weather is currently " + description + "</p >")
      res.write("<h1>The temperture in " + query + " is " + temp + "degrees Celcius.</h1>")
      res.write("<img src =" + imageURL + ">")
      res.send()
    })
  })

  console.log()
})




app.listen(3000, function () {
  console.log("Server is running on port 3000.")
})
```

Project Setup

```js
const express = require("express")
const bodyParser = require("body-parser")
const request = require("request")


const app = express()

app.get("/", function (req, res) {
  res.send("Server is up and running")
})



app.listen(3000, function () {
  console.log("Server is running on port 3000.")
})
```

## Newseletter Project

```js
const express = require("express")
const bodyParser = require("body-parser")
const request = require("request")


const app = express()

app.use(express.static("public")) //use to identify a static folder, inside html do not need to include this static folder

app.use(bodyParser.urlencoded({ extended: true }))

app.get("/", function (req, res) {
  res.sendFile(__dirname + "/signup.html")
})



app.listen(3000, function () {
  console.log("Server is running on port 3000.")
})
```

# Git and GitHub

## Version control

`ls -a` show all the hidden files in the folder

`git init` able to init locally and able to go back show the version control and many operations

`git status` show the untracked file or the new changes on the file

`git commit -m "<commit message>"`

`git log` show the commit information

`git add .` add all files inside the folder

`git diff <filename>`, show the difference between two files

`git checkout <filename>` go back to the last checkpoint version

`git remote add <origin> + url`



working directory -> `git add` staging area ->`git commit` local repository - master branch/ main branch

.git

git push -> Remote repository -> GitHub

## Push to Github

`git remote add origin  <REMOTE_URL> ` the github repo url

`git push -u origin main` push the changes in your local repo to the remote repo

## Gitignore

`touch .gitignore.` in your local repo

`git rm --cached -r .` remove every files from staging area to local

## Cloning

`git clone + url`

## Branching and Merging

`git branch <name>`

`git branch` show branch

`git checkout <branch name>` switch to branch alien-plot

`git log` [press q to exit]

`git merge branch name`

`:q!` to save merge and quit

//https://learngitbranching.js.org/ // git challenge and learning website

![Screen Shot 2022-08-13 at 5.49.59 PM](/Users/richardqiu/Library/Application Support/typora-user-images/Screen Shot 2022-08-13 at 5.49.59 PM.png)

![Screen Shot 2022-08-13 at 5.52.23 PM](/Users/richardqiu/Library/Application Support/typora-user-images/Screen Shot 2022-08-13 at 5.53.01 PM.png)

## Forking and Pull Request

Forking - 

Pull Request, 

![Screen Shot 2022-08-13 at 6.23.23 PM](/Users/richardqiu/Library/Application Support/typora-user-images/Screen Shot 2022-08-13 at 6.23.23 PM.png) 

Git cheat sheet most commands:[atlassian-git-cheatsheet.pdf](../../Downloads/atlassian-git-cheatsheet.pdf) 

# EJS

Embedded Javascript templating

## Templates

//url = https://github.com/mde/ejs/wiki/Using-EJS-with-Express by using express

<%= variable %>



## Scope

For if,for,while loop conditional statements,

`var`	global, that can be accessed 

`let`	local

`const`	also local

much safer to use `let` and `const` in javascript code

## Layout





## Blog Website

## Foreach

In js, the foreach() function can printout every function in the array function

const array1 = ['a', 'b', 'c'];

array1.forEach(element => console.log(element));

## Loadash library



# Database

## SQL

Structured Query Language(sequel) - MySQL,PostgreSQL

Need to follow the specific structure, empty element will have null

MySQL is a table-based system 

- Relational
- More Mature
- Table Structure
- Requires a Schema
- Great with Relationships
- Scales Vertically

## NoSQL

Not only structured query language - mongoDB, pedis

No need to follow the specific structure

- Non-Relational
- Shiny and New
- Document Structure
- More Flexible to Changes
- Not Great with Complex Relationships
- Horizontally Scalable



## SQL

https://www.w3schools.com/sql/

- Create 
- Read
- Updata
- Destroy

## CRETE TABLE and INSERT DATA, FOERGIN KEY, INNER JOIN

```sql
INSERT INTO table_name
VALUES (value1, value2, value3, ...);

INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...);

CREATE TABLE orders (
    id INT NOT NULL,
    order_number INT,
  	customer_id INT,
  	product_id INT,
  	PRIMARY KEY(id)
  	FOREIGN KEY()
);
```



## READ,SELECT, and WHERE

```sql
SELECT column1, column2, ...
FROM table_name
WHERE id=1; //condition
```

## Upadate Single Values

```sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

## Update by Adding a Column

```sql
ALTER TABLE table_name
ADD column_name datatype;
```

## Delete

```sql
DELETE FROM table_name WHERE condition;
```



# MongoDB

## CRUD(MongoDB Shell)

https://www.mongodb.com/docs/mongodb-shell/run-commands/

To run commands in `mongosh`, you must first [connect to a MongoDB deployment](https://www.mongodb.com/docs/mongodb-shell/connect/#std-label-mdb-shell-connect).

Create

`use databse`

Update

`db.products.updateOne({_id:1},{$set:{stock:32}})`

```
db.products.insertOne({
	_id:2,
	name:"pencil",
	price:0.80,
	stock:12,
	review:[
	{
		authorName:"Sally",
		rating:5,
		review:"Best pencil ever!"
	},
	{
		authorName:"John",
		rating:5,
		review:"Awesome pencil",
	}
	]
})
```

Delete database

`use database`

`db.dropDatabase()`



## Mongoose

ODM. Object Document Mapper

```js
const mongoose = require('mongoose')
mongoose.connect('mongodb://localhost:27017/fruitsDB')

const fruitSchema = new mongoose.Schema({
  name: String,
  rating: Number,
  review: String
})

const Fruit = mongoose.model("Fruit", fruitSchema) //note that mangoose will automatically let fruit become plurals
//https://stackoverflow.com/questions/10547118/why-does-mongoose-always-add-an-s-to-the-end-of-my-collection-name

const fruit = new Fruit({
  name: "Apple",
  rating: 7,
  review: "Pretty solid as a fruit"
})

//fruit.save()

const Personschema = new mongoose.Schema({
  name: String,
  age: Number
})
const Person = mongoose.model("Person", Personschema)

const person = new Person({
  name: "John",
  age: 17
})

person.save()

const kiwi = new Fruit({
  name: "Kiwi",
  rating: 7,
  review: "Pretty solid as a fruit"
})
// Fruit.insertMany([kiwi], function (error, docs) { })
Fruit.find(function (err, fruits) {
  if (err) {
    console.log(err)
  } else {
    console.log(fruits)
    fruits.forEach(function (fruit) {
      console.log(fruit.name)
    })
    mongoose.connection.close()
  }
})
```

## Locally

First step: 

1. Connect to the mongoose server `mongosh`

2. To use mongoose, install `npm i mongoose` in your project

3. ```json
   const mongoose = require("mongoose")
   
   //database
   mongoose.connect('mongodb://localhost:27017/blogContent')//connect to your default local envrionment and create or find a database called blogContent
   
   const postSchema = new mongoose.Schema({
     title: String,
     content: String
   }) //
   //define a schema
   
   const Post = mongoose.model("Post", postSchema) //"Post" is a collection of the database
   //define a model
   
   
     const post = new Post({
       title: req.body.postTitle,
       content: req.body.postBody
     })
     //add documents into your collections
     post.save(function (err) {
       if (!err) {
         res.redirect("/")
       }
    }//save your documents at the end
   
   ```

## Deploying Apps with Databases

Heroku to store 

MongoDb to store the database

# RESTful Api

Representational State Transfer

HTTP Request - Hypertext Transfer Protocal request

HTTPS stands for secure request

FTP Request



RESTful Api - An architectural style for designing APIs 

HTTP Verbs - GET, Post, Put, Patch, Delete

GET - READ

POST - CREATE

PUT,PATCH - Update database

PUT-update by setting an entire entry

PATCH - update a piece of data that need to be updated



# Authentication

Level 1

Level Database encryption, unscramble it, 给密码加密

Level 2 - Encryption

Encrypt by using mongoose-encryption" and dotenv npm package.

Level 3 - Hashing

Password -> Hash function -> Hash 

Two same string passing the hash function will have same output, using this property to check if have the same input.

Level 4 - Hashing & Salting

Industry standard 17,00 berypt Hashes/Second

## What are cookies and sessions





# React

## JSX & es6 in react

use a curly braces `{ variable }` to use a variable `{js scripts can be written in here}`, can write expressions but can't write statements

In JSX, img in js need to have a closing tag

`<img` src = {img} `/>`

Use classname instead of class in js to use the css style sheet.

## Inline Styling 

```react
const customStyle = {
  color: "red",
  fontSize: "20px",
  border: "1px solid black"
};

customStyle.color = "blue";

ReactDOM.render(
  <h1 style={customStyle}>Hello World!</h1>,
  document.getElementById("root")
);

```

Practise with inline and Function and className

```react
//Create a React app from scratch.
//Show a single h1 that says "Good morning" if between midnight and 12PM.
//or "Good Afternoon" if between 12PM and 6PM.
//or "Good evening" if between 6PM and midnight.
//Apply the "heading" style in the styles.css
//Dynamically change the color of the h1 using inline css styles.
//Morning = red, Afternoon = green, Night = blue.
import React from "react";
import ReactDOM from "react-dom";

var time = new Date().getHours();

function Time(currentTime) {
  if (currentTime < 12 && currentTime > 0) {
    return (
      <h1 className="heading" style={{ color: "red" }}>
        Good morning{" "}
      </h1>
    );
  } else if (currentTime < 18) {
    return (
      <h1 className="heading" style={{ color: "green" }}>
        Good Afternoon{" "}
      </h1>
    );
  } else {
    return (
      <h1 className="heading" style={{ color: "blue" }}>
        Good evening{" "}
      </h1>
    );
  }
}
ReactDOM.render(<Time currentTime={time} />, document.getElementById("root"));

```



## React Components



Export js, export { } do matter when import in index.js script, need to have the same name, thehe  default name doesn't need to be the same

## Property

## Mapping

Mapping function can be used to directly mapped all elements by using a function
