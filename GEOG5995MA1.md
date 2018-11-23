<html>
<head>
<style>
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #333;
}

li {
    float: left;
}

li a, .dropbtn {
    display: inline-block;
    color: white;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
}

li a:hover, .dropdown:hover .dropbtn {
    background-color: #FFA500;
}

li.dropdown {
    display: inline-block;
}

.dropdown-content {
    display: none;
    position: absolute;
    background-color: #f9f9f9;
    min-width: 160px;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    z-index: 1;
}

.dropdown-content a {
    color: black;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
    text-align: left;
}

li a.active {
    background-color: #FFA500 ;
    color: white;
}

.dropdown-content a:hover {background-color: #FFA500}

.dropdown:hover .dropdown-content {
    display: block;
}

</style>
</head>

<body>
<ul>
  <li><a href="index.html">About Me</a></li>
  
  <li class="dropdown">
    <a href="javascript:void(0)" class="dropbtn">GEOG5995M</a>
    <div class="dropdown-content">
      <a class = "active" href="#">Assignment 1</a>
        <a href="GEOG5995MA2.html">Assignment 2</a>
    </div>
  </li>
    <li class="dropdown">
    <a href="javascript:void(0)" class="dropbtn">SLSP5301M </a>
    <div class="dropdown-content">
      <a href="#">Assignment 1 and 2</a>
        <a href="#">Assignment 3</a>
    </div>
  </li>
    </li>
    <li class="dropdown">
    <a href="javascript:void(0)" class="dropbtn">MM8040</a>
    <div class="dropdown-content">
      <a href="#">Assignment 1</a>
        <a href="#">Assignment 2</a>
          <a href="#">Assignment 3</a>
            <a href="#">Assignment 4</a>
              <a href="#">Assignment 5</a>
    </div>
  </li>
  <li><a href="https://datacdt.org/">News</a></li>
</ul>

</body>

</html>

## Assignment 1

The project [brief](http://www.geog.leeds.ac.uk/courses/computing/study/core-python-phd/assessment1/index.html) outlined the aims for the assignment. The main aim was to create an online portfolio of my practial work. 

This page displays my code, including a downloadable link, as well as other interesting parts of my Agent-based model (ABM).

The image is a compilation of sequential snapshots of my ABM at different frames.
![image](Webp.net-gifmaker.gif)


To begin, I created my _agentframwork_ class. This class was called *Agent* which includes a set of behavioural rules governing my agents and their environment.

I started with the initialisation function:

```
import random

class Agent:

def __init__(self, environment, agentlist):
        '''The init function serves as the constructor and self represents the instance of the object itself.
           So here I'm constructing an environment and a list of agents''' 
        self.columny = (random.randint(0,99))
        self.columnx = (random.randint(0,99))
        '''I set the generation of (y,x) columns to random and between 0-99''' 
        self.environment = environment
        self.agentlist = agentlist
        self.store = 0
        '''The objects: environment, agentlist and store were also created at this point'''
```
Following the initialisation, I have a starting ground and can begin to build after the creation of my objects. 

Before we proceed, I'll define all the objects used in this ABM for clarity.

| Object        | Definition    | 
| ------------- |:-------------:| 
| Environment   |  |
| Agentlist     | A list of all agents within my model |
| columny/x     | Columns which include a list of randomly generated numbers between 0-99  |
| Store         | Storage of resources agents accumulate from the environment or neighbours|
|    |  |

The next step was to define how my agents could move in the Environment.

```
