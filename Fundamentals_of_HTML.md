# HTML Elements
<p>HTML is made up of elements. General makeup of a HTML element looks like the following:

![image](https://user-images.githubusercontent.com/110134426/182184380-05bb8c6f-ea11-4a4d-8994-b999c1a0064a.png)

<br>
<p>A commonly used tag is the <strong>body tag</strong>. This is represented by an opening tag: < body > and a closing tag < /body >.
<br>Only content inside the opening and closing body tags can be displayed to the screen.

***

#### HTML Structure
<p> A child element is when one element is contained inside another, for example a < p > tag inside the < body > tag.

![image](https://user-images.githubusercontent.com/110134426/182185011-2069bc38-fb34-4ac3-b126-5332611aa679.png)

***
#### HTML Headers
<p>In HTML, there are six different headings, or heading elements.
<br><ul>
   <li>< h1 > = Main Heading
   <li>< h2 > = Sub Heading
   <li>< h3 > = Sub Sub Heading
   <li>< h4 >
   <li>< h5 >
   <li>< h6 >
</ul>
These headings have to be used with an escape tag e.g. < /h1>

***

#### HTML Div
<p>One of the most popular elements in HTML is the < div > element. < div > is short for “division” or a container that divides the page into sections.

![image](https://user-images.githubusercontent.com/110134426/182187489-f8efb1f6-8ff9-4bf7-888e-58e4ef248a5b.png)

Divs don't have any distinguishing visual feature but are useful for when you want to apply different formats to sections on your page.</p>

***

#### HTML Attributes
If we want to expand an element’s tag, we can do so using an attribute. 
Attributes are content added to the opening tag of an element and can be used in several different ways, from providing information to changing styling. 
<br>Attributes are made up of the following two parts:

+ The name of the attribute.
+ The value of the attribute.
The id attribute is used to specify differences between elements for example, different Div elements.

***

#### Displaying Text
In order to display text on a page you use 'paragraph' or 'span'
+ Paragraphs (< p >) contain a block of plain text.
+ < span > contains short pieces of text or other HTML. They are used to separate small pieces of content that are on the same line as other content.
It’s best to use a < span > element when you want to target a specific piece of content that is inline, or on the same line as other text.


![image](https://user-images.githubusercontent.com/110134426/182187992-eef00a6f-2660-49df-b26f-12ff0880b27a.png)

***

#### Styling Text
For italics use < em >
<br>For bold use < strong >

![image](https://user-images.githubusercontent.com/110134426/182188289-b4adce27-7c26-429f-97de-47c0f7cb3f4c.png)

***

#### Line Breaks
<p>In order to create a line break, use < br >. There is no need to use a closing tag with this element.
<p>These can be doubled up in order to create multiple consecutive line breaks

***

#### Lists
<p> < ul > is used to create an Unordered List
<p>This list is **bulleted**
<p> < li > is used to add items that list (this must be a child to the < ul > list

![image](https://user-images.githubusercontent.com/110134426/182188372-ad1cd312-1130-417a-8562-167d9410079d.png)

<p> < ol > is used to create an Ordered List
<p>This list is **numbered**
<p> the same < li > element as unordered lists is used to enter elements into it.

![image](https://user-images.githubusercontent.com/110134426/182188387-76558b94-811f-4bc2-ae8b-3844876e06ce.png)

***

#### Images
<p>In order to add an image use the following syntax:
<p>< img scr="URL" />

![image](https://user-images.githubusercontent.com/110134426/182188441-730852ac-9fed-4a50-92a8-8e5b3f7601a4.png)

<p>To add a tag to your image use the "alt" attribute:

![image](https://user-images.githubusercontent.com/110134426/182188476-a2494274-49c4-48f9-8e05-542088ca286a.png)

***

#### Videos
<p>Videos are similar to images however a video element **requires a closing tag**
<p>"width" and "height" are also required elements
<p>"controls" is used to tell the browser to include basic stop/start video controls
<p>Lastly, text can be included between the tags to show if the video is unable to load

![image](https://user-images.githubusercontent.com/110134426/182188527-8fc89754-a2b4-4f8c-906e-f306db08480d.png)

***

## HTML: Structure
#### Document Type Declaration
<p>In order to tell the browser that you are using HTML, you need to start with a document type declaration:

![image](https://user-images.githubusercontent.com/110134426/182188573-1d4fe91e-f769-41ff-85b6-cad70650d0fd.png)
  
***

#### HTML Tag
Next, in order to create HTML structure and content you need to create a HTML open and closing tag:

![image](https://user-images.githubusercontent.com/110134426/182188606-7ef7acfa-e23b-44da-8afc-9d8e1d94499e.png)

***
  
#### Head Element
The < head > element contains the metadata for a web page. Metadata is information about the page that isn’t displayed directly on the web page.</br>
For example, the < title > of the webpage will be housed insie the head element
  
![image](https://user-images.githubusercontent.com/110134426/182189357-22c65689-40ca-472e-8640-4c68373a6069.png)

***
  
#### Linking to Other Webpages
  Use an anchor element < a > to include a link to another wesite.</br>
  Use the following syntax:
  
  ![image](https://user-images.githubusercontent.com/110134426/182190651-0213af0b-a57f-4cfc-a90d-e90f4bf9699c.png)
  
  To open a link in a new window, set the "target" attribute to equal <strong>"_blank":</strong>
  
  ![image](https://user-images.githubusercontent.com/110134426/182194227-ec028d22-2a40-4383-8e36-77b29d0518bd.png)

  You can turn any element onto your page into a hyperlink by wrapping it in an achor element i.e. images:
  
  ![image](https://user-images.githubusercontent.com/110134426/182196397-2c1db8ed-4223-46c1-85f4-b521152ddc23.png)

***

#### HTML Comments
  <p>Comments begin with < !--</P>
  <p>...and end with -- ></P>

***
# Brown Bear Project
  
***
  
<!DOCTYPE html>
<html>

<head>
  <title>Brown Bears</title>
</head>

<body>
  <nav>
    <a href="./index.html">Brown Bear</a>
    <a href="./aboutme.html">About Me</a>
  </nav>
  <h1>The Brown Bear</h1>
  <nav>
    <ul>
      <li><a href="#introduction">Introduction</a></li>
      <li><a href="#habitat">Habitat</a></li>
      <li><a href="#media">Media</a></li>
    </ul>
  </nav>
  <div id="introduction">
    <h2>About Brown Bears</h2>
    <p>The brown bear (<em>Ursus arctos</em>) is native to parts of northern Eurasia and North America. Its conservation status is currently <strong>Least Concern</strong>.<br /><br /> There are many subspecies within the brown bear species, including the
      Atlas bear and the Himalayan brown bear.</p>
    <a href="https://en.wikipedia.org/wiki/Brown_bear" target="_blank">Learn More</a>
    <h3>Species</h3>
    <ul>
      <li>Arctos</li>
      <li>Collarus</li>
      <li>Horribilis</li>
      <li>Nelsoni (extinct)</li>
    </ul>
    <h3>Features</h3>
    <p>Brown bears are not always completely brown. Some can be reddish or yellowish. They have very large, curved claws and huge paws. Male brown bears are often 30% larger than female brown bears. They can range from 5 feet to 9 feet from head to toe.</p>
  </div>
  <div id="habitat">
    <h2>Habitat</h2>
    <h3>Countries with Large Brown Bear Populations</h3>
    <ol>
      <li>Russia</li>
      <li>United States</li>
      <li>Canada</li>
    </ol>
    <h3>Countries with Small Brown Bear Populations</h3>
    <p>Some countries with smaller brown bear populations include Armenia, Belarus, Bulgaria, China, Finland, France, Greece, India, Japan, Nepal, Poland, Romania, Slovenia, Turkmenistan, and Uzbekistan.</p>
  </div>
  <div id="media">
    <h2>Media</h2>
    <img src="https://content.codecademy.com/courses/web-101/web101-image_brownbear.jpg" />
    <video src="https://content.codecademy.com/courses/freelance-1/unit-1/lesson-2/htmlcss1-vid_brown-bear.mp4" height="240" width="320" controls>Video not supported</video>
  </div>
</body>

</html>
  
  
  
  
  
  
  
  
  
  
  
  
  
