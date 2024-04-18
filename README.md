# Ex04 Places Around Me
## Date: 15-04-2024

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE
```<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Map</title>
</head>
<style>
    *{margin: 0;}
</style>
<script>
    function coordinate(event){
        let x=event.clientX;
        let y=event.clientY;
        document.getElementById("text1").value=x;
        document.getElementById("text2").value=y;
    }
</script>
<body>
    <img src="map image.jpeg" width="1000" height="500" usemap="#MapNew" onmousemove="coordinate(event)" >
    <map name="MapNew">
        <area shape="rect" coords="110,404,182,425" href="https://simatsengineering.com/" title="Saveetha School of Engineering">
        <area shape="rect" coords="1,431,80,450" href="https://www.saveetha.ac.in/" title="Saveetha Engineering College">
        <area shape="rect" coords="736,100,815,122" href="https://sapoly.edu.in/courses/" title="SA Polytechnic College">
        <area shape="rect" coords="932,95,996,117" href="https://www.sindhicollege.com/" title="Sindhi College">
        <area shape="rect" coords="854,24,930,47" href="https://www.shenbaghacollegeofnursing.org/" title="Shenbaga College of Nursing">
        <area shape="rect" coords="60,372,139,395" href="https://www.libartssaveetha.com/" title="Saveetha College of Liberal Arts">
    </map><br>
    X-coordinate <input type="text" id="text1">
    <br><br>
    Y-coordinate <input type="text" id="text2">
    
</body>
</html>```


## OUTPUT
![Screenshot 2024-04-15 191619](https://github.com/ssonuma/NearMe/assets/150653312/787b7e4a-e040-4246-bd6f-1b5a3b8d0ecb)







## RESULT
The program for implementing image maps using HTML is executed successfully.
