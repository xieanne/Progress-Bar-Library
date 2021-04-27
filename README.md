# Progress Bar Library (Anne Xie)

Progress Bar Library is a library that has different types of progress bars that aims to help developers to make their websites more visually appealing and able to present the numbers more dynamically.

If want to go back to the home page, simply press the top left corner's title
<br />
Link to demo: https://various-progress-bars.herokuapp.com/
<br />
Link to API documentation: https://various-progress-bars.herokuapp.com/api.html

## Get Started
Links that needs to be included:
```
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
<link rel="stylesheet" href="style.css">
```

Scripts that needs to be included:
```
<script defer src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script defer type="text/javascript" src='ProgressBar.js'></script>
```

Instantiation of a progress bar object:
```
const pb = new ProgressBars();
```

Example of an API call:
```
const DOMToAppendTo = document.getElementById("someID");
    
const configure = {
    eventSpecified: "load",
    withPercentage: false,
    desired_percentage: 100,
    increasing_speed: 20,
    type: "filled",
    withPattern: false,
}

const style = {
    width: "80%",
    marginTop: "20px",
    marginLeft: "0px",
    backgroundColor: "#c5cae9",
    barColor: "#5c6bc0",
    borderRadius: "20px",
    height: "30px",
    borderHeight: "20px",
    percentagePosition: "90%",
    percentageColor: "black"
}
pb.makeProgressBar("regularProgressBar", configure, style, DOMToAppendTo);
```
            
