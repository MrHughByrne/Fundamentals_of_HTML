# Fundamentals of HTML: 4/5 Tables & 5/5 Semantics
## Tables
In order to create a table, we use < table > and </ table ></br>
This will be created in the "body" element.</br>

***

### Rows
The first step in entering data into the table is to add rows using the table row element: < tr >.

![image](https://user-images.githubusercontent.com/110134426/182213189-84c72fa5-ee4c-4a14-8322-200414f3e717.png)

Within these rows, to add the data to each cell use the following < td > syntax:

![image](https://user-images.githubusercontent.com/110134426/182213933-86232e29-a630-42b0-a207-0be0ade0aace.png)

***

### Table Headings
To add headings to each row and column, we use < th > <br>
Just like table data, the table heading needs to be placed within the table row

![image](https://user-images.githubusercontent.com/110134426/182214363-5c938c4b-a6d5-4e80-a7bb-86455a1c31bd.png)

In the above table:</br>
+ "row" makes it clear that the heading is for a row
+ "col" makes it clear that the heading is for a column
+ 
***

### Table Borders
The HTML method for creating table borders is deprecated. Nowadays, CSS is used for styling tables.<br>
The below HTML uses the "border" attribute where the integer represents the border thickess:

![image](https://user-images.githubusercontent.com/110134426/182220096-e9b9d79c-09e2-43a5-aa78-ee0bb776ac43.png)

The below is the CSS equivalent:

![image](https://user-images.githubusercontent.com/110134426/182219995-85e64af7-9dfe-4ce2-8dfc-3001af69e51d.png)

***

### Spanning Columns
If you have data that spreads across multiple columns e.g. calendar event, you can use "colspan"</b.
This accepts an integer which represents the number of columns it spans across

![image](https://user-images.githubusercontent.com/110134426/182221175-8458e822-d3f2-4995-8afc-3dae6a515613.png)

***

### Spanning Rows
Similar to colspan, "rowspan" is used to span across multiple rows e.g. an event that goes for multiple hours

![image](https://user-images.githubusercontent.com/110134426/182222700-d5ed24ea-779e-4507-93b3-c9bef1b41326.png)

Here's what the table looks like with spanned rows and columns:

![image](https://user-images.githubusercontent.com/110134426/182223191-ff2ed639-e29c-4aec-960d-29e6370ef09c.png)

***

### Table Sections
The code for a table can be broken up into sections, similar to the "Div" Element
<ol>
  <li>< thead > can be used to house the title row of columns</li>
  <li>< tbody > can be used to house the data of the table</li>
  <li>< tfoot > can be used to house the footer of the data (e.g. summed results of the table)</li>
  
***
  
## Summary

![image](https://user-images.githubusercontent.com/110134426/182228623-f40bf3ff-5f0c-4842-a8b7-391c2b534424.png)

## Project: Wine Festival Website
  
Link: https://content.codecademy.com/courses/learn-html-tables/index.html

<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <title>Aguillar Family Wine Festival</title>
  <link rel="stylesheet" type="text/css" href="reset.css" />
  <link rel="stylesheet" type="text/css" href="style.css" />
  <link href="https://fonts.googleapis.com/css?family=Oswald" rel="stylesheet">
</head>

<body>
  <header>
    <h1>Annual Aguillar Family Wine Festival</h1>
  </header>
  
  <div class="container">
    <table>
      <thead>
        <tr>
          <th scope="col1" colspan="2"><h1>Wine Festival Schedule</h1></th>
        </tr>
        <tr>
           <th scope="col2"><h2>Time</h2></th>
           <th scope="col2"><h2>Event</h2></th>
        </tr>
      </thead>
      <tbody>
        <tr> <!-- Row 1 -->
          <td class="left"><h3>12:00PM</h3></td>
          <td><h3>Welcome Reception</h3></td>
        </tr>
        <tr> <!-- Row 2 -->
          <td class="left"><h3>01:00PM</h3></td>
          <td><h3>Storytelling & Tasting</h3></td>
        </tr>
        <tr> <!-- Row 3 -->
          <td class="left"><h3>02:00PM</h3></td>
          <td><h3>Wine Luncheon</h3></td>
        </tr>
        <tr> <!-- Row 4 -->
          <td class="left"><h3>03:00PM</h3></td>
          <td><h3>Aguillar Family Wines</h3></td>
        </tr>
        <tr> <!-- Row 5 -->
          <td class="left"><h3>04:00PM</h3></td>
          <td><h3>Wine & Cheese Tasting</h3></td>
        </tr>
      </tbody>
    </table>
  </div>
  
  <footer>
    <h3>Contact</h3>
    <h3>Location</h3>
    <h3>Privacy Policy</h3>
  </footer>
</body>

</html>
