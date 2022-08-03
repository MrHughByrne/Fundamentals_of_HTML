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

***
 ## Semantic HTML

Structure elements of HTML
#### Header
+ < header >  a container usually for either navigational links or introductory content containing < h1 > to < h6 > headings.
  <br></br>
![image](https://user-images.githubusercontent.com/110134426/182596533-008e5179-a7b2-4603-b672-46a7c1d7b1bd.png)

***

#### Footer
  + < footer > content at the bottom of the subject information</br>
  <br></br>
![image](https://user-images.githubusercontent.com/110134426/182596569-f1bab9b0-efcd-469d-a4fd-4385feeedb09.png)

***

#### Main
  + < main > used to encapsulate the dominant content within a webpage.</br>
  <br></br>
![image](https://user-images.githubusercontent.com/110134426/182596592-42cd781f-ad14-4a3f-86a7-86a70305800e.png)

***

#### Nav
+ < nav > used to define a block of navigation links such as menus and tables of contents.
  <br></br>
![image](https://user-images.githubusercontent.com/110134426/182597050-c79a0ec1-1ef8-44d0-ac00-2a959a7d509c.png)

***

#### Section
+ < section > defines elements in a document, such as chapters, headings, or any other area of the document with the same theme.
  <br></br>
![image](https://user-images.githubusercontent.com/110134426/182597073-5b4053bf-031d-44f7-a1a8-702583dcbab9.png)

***

#### Article
+ < article > element holds content that makes sense on its own.
  <br></br>
![image](https://user-images.githubusercontent.com/110134426/182597162-bb7781db-1e3f-45be-932d-f039b1650d49.png)

***

#### Aside
+ < aside > element is used to mark additional information that can enhance another element but isn’t required in order to understand the main content. This element can be used alongside other elements such as < article > or < section >. 
   <br></br>
![image](https://user-images.githubusercontent.com/110134426/182597189-72c537fc-4d5c-4c17-92dc-50620801c526.png)

***

#### Figure
+ < figure > is an element used to encapsulate media such as an image, illustration, diagram, code snippet, etc, which is referenced in the main flow of the document.
  <br></br>
![image](https://user-images.githubusercontent.com/110134426/182597215-e188cf40-be2e-4ae6-a2e7-86b05524443c.png)

***

#### Figcaption
+ < figcaption > is an element used to describe the media in the < figure > tag.
  <br></br>
![image](https://user-images.githubusercontent.com/110134426/182597291-73de8f94-c6fb-4a62-a225-de968394ef9a.png)

***

#### Audio
+ < audio > element is used to embed audio content into a document.
  <br></br>
![image](https://user-images.githubusercontent.com/110134426/182597345-7e128be6-d818-4472-a360-82b9d85369bd.png)

+ Within the audio element, we can also call for "controls" which will automatically display the audio controls into the browser such as play and mute.
  <br></br>
![image](https://user-images.githubusercontent.com/110134426/182597420-28e82c9d-a371-41fe-9f6f-0b6e2117aad9.png)

***

#### Video
+ < video > allows you to add videos to your website
  <br></br>
  ![image](https://user-images.githubusercontent.com/110134426/182597834-b5cf4b38-a7bc-42f5-b2fe-695cad24e42b.png)

***
  
#### Embed
+ < embed > embeds any media content including videos, audio files, and gifs from an external source.
  <br></br>
  ![image](https://user-images.githubusercontent.com/110134426/182598123-b1400ccb-9c8c-405b-8dca-ecb4303970f0.png)


  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
