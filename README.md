# week9

The goal is to build a website with Bootstrap that fetches and displays one of two graphs.

Step 1: Bootstrap setup

Create a normal HTML page named index.html
Go to getbootstrap.com and import the CSS and Js files for Bootstrap to your HTML page
Utilize the Navbar and jumbotron components
The navbar should have 2 buttons on it, each with a unique ID: one for pie and one for line
The jumbotron should instruct the user to use the buttons in the navbar to toggle graphs
 

Step 2: Fetch data

When the page loads, you'll make two network requests
One to get the 'gameHours' API
One to get the 'stressSource' API
You'll create 2 functions: "createPieChart" and "createLineGraph" that will accept data to display
For each fetch request, when the data comes back, you'll want to call the above functions with the returned data from the API
 

Step 3: Create graphs

Using the Line graph (https://canvasjs.com/html5-javascript-line-chart/ (Links to an external site.)) and the Pie chart (https://canvasjs.com/html5-javascript-pie-chart/ (Links to an external site.)) documentation, create both graphs
The "dataPoints" of both graphs should be provided by the data from the APIs
https://github.com/MUFall2020-BIT240/professor_api (Links to an external site.) has the endpoints detailed
The div that contains the graph for the pie chart should have 'display: none;' on it via CSS so that only the line graph is visible at first
Add event listeners to the buttons in the navbar that call functions "showPieChart" and "showLineGraph"
Each of those functions should use jQuery $().show() (Links to an external site.) and $().hide() (Links to an external site.) to make sure only the requested graph is present. 
