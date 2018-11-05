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

The project [brief](http://www.geog.leeds.ac.uk/courses/computing/study/core-python-phd/assessment1/index.html) outlined the aims for the assignment.

The first part of the assignment was to attach my ABM created during the training course, and secondly was to create this website to display my output. 

