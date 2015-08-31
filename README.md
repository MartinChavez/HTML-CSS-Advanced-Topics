<a name="README"><img src="http://static1.squarespace.com/static/54b6c223e4b0ad6fb5d5569b/t/54bec5a4e4b0c74e7f3b09e9/1421788582011/large_html.jpg" width="300px" height="200px"/></a>

# HTML5/CSS3: Annotated tutorial

Use this tutorial as a guide to learn HTML5 and CSS3. Each unit contains an annotated lesson that can assist you in developing your Web Development skills.

Topics
================
 - Basics
 - Divs
 - Fonts
 - Hexadecimal Colors
 - Images
 - Links
 - Selectors
 - The Box Model
 - Web Forms
 
HTML Basics
====================
```HTML
<!--HTML: Basics-->

<!--HTML: HyperText Markup Language -->
<!--HTML is the standard markup language used to create web pages-->

<!-- To add content, you should use HTML tags -->
<!-- These pre-defined tags, have opening and closing versions -->


<!-- <!DOCTYPE> tag -->
<!-- Defines the HTML Version the browser should use to display the HTML Tags-->
<!-- By writing <!DOCTYPE html> and not specifying the version, the browser will use the latest version-->
<!DOCTYPE html>


<!-- <html> tag -->
<!-- All of the HTML tags are placed inside the <html> tag -->
<!-- You should use it to organize all of the other tags for the Web Page -->
<html>

<!-- <head> tag -->
<!-- All the not-visible content of the web page should be contained on the <head> tag -->
<!-- You can use this tag to load scripts like CSS and Javascript -->

<!-- Nesting tags: HTML tags can contain other tags -->
<head lang="en"><!-- the <head> tag is called the parent tag (for <meta> and <title>) -->
    <meta charset="UTF-8">
    <!-- the <meta> tag is called a children tag (of <head>)-->
    <title>HTML Basics</title><!-- the <title> tag is called a children tag (of <head>) -->
</head>

<!-- <link> tag -->
<!-- Allows you to reference other files that work together with this file-->

<!-- The type attribute set to text/css lets the browser know you are loading a CSS file -->
<!-- The 'rel' attribute is an abbreviation for 'relationship' -->
<!-- The CSS selectors and rules are contained in the CSS file -->
<link rel="stylesheet" type="text/css" href="../CSS/Basics.css"><!-- The <link> is an empty tag, it doesn't have a closing tag -->


<!-- <body> tag -->
<!-- All the visible content of the web page should be contained in the <body> tag -->
<body>

<!-- <h*> headers -->

<!-- You can use heading tags to define your content hierarchy -->
<!-- Higher heading numbers mean the content that appears between the tags is less important -->

<!-- <h1> is an opening tag -->
<h1>Header H1</h1>
<!-- </h1> is an closing tag and has a slash before the tag name-->
<h2>Header H2</h2>

<h3>Header H3</h3>
<h4>Header H4</h4>

<!-- <p> paragraphs -->

<!-- You can use paragraph tags for non-heading text -->
<p>This is a paragraph</p>
<p>This is another paragraph</p>

<!-- <ul> Unordered List -->
<!-- You can use unordered list tags to display a list fo items -->
<ul>
    <!-- <li> list item -->
    <!-- Every list item needs to be put in a <li> tag -->
    <li>List Item 1</li>
    <li>List Item 2</li>
    <li>List Item 3</li>
</ul>

<!-- <ol> Ordered List -->
<!-- You can use ordered list tags to display a list of items in order -->
<ol>
    <!-- <li> list item -->
    <!-- Every list item needs to be put in a <li> tag -->
    <li>List Item 1</li>
    <li>List Item 2</li>
    <li>List Item 3</li>
</ol>
```
CSS Basics
====================
```CSS
/* CSS */

/* CSS is the language for describing the presentation of HTML elements */

/* Selectors*/
/* CSS elements that allow you to find HTML elements */

/* Selectors: Type*/
/* You can create a Type selectors by writing the tag name without <> brackets */
p {
    text-overline: 3;/* You can change any property of the tag */
}

/*Selector: Syntax*/
/*
selectorName {
    property: value;
}
*/

/* A single selector can change multiple properties*/
p {
    text-overline: 3;
    text-underline: dot-dash;
    color: red;
}

/* Selectors will select all matching tags on the page and apply the properties*/

/* Descendant Selectors */
/* They can be used to select tags only if they are children of another tag*/

ul li {
    font-size: 30px;
    color: darkgreen;
}

/* Pseudo Selectors*/
/* Pseudo-selector is a modifier that can be added to a selector to select a tag
only when a certain condition has occurred */
ul li:hover{
    color: pink;
}

/* Pseudo Selector: First Child*/
/* The :first-child pseudo-selector can be applied to narrow the amount of children selected */
ol li:first-child{
    color: lightcoral;
}
```

The Box Model
====================
```CSS
/* The Box Model */

/*Every tag shown in the body is contained in an invisible rectangle called Box*/
/*The box model is a way to describe the borders and spacing in between the boxes of each tag*/

/*Block-level tags*/

/*The content of block-level tags take up the entire width (horizontal space) of the container*/
/*Every box is pushed to the line below*/

/*Examples of block-level tags : */
/* h1 , h2,  h3,  p,  ul,  li*/

/*Inline-level tags*/
/*Every tag that is not block-level, is called inline-level/
/*The content of these tags do not take the entire width of the container */

/*Examples of inline-level tags: */
/* a, img , input, label*/

/*Converting block-level tags into inline-level tags*/
/*Allow you to display items horizontally instead of vertically*/

ul li {
    display: inline;
}

/*Box Model Parts*/

/*Content area*/
/*Contains the actual content (text, images, etc.)*/
/*It will take up as much vertical space as it needs to display the content inside*/

/*Padding*/
/*Padding is a layer on every edge of the content area*/
/*Padding can be added to the top, right, bottom or left of the content area*/

/*Border*/
/*Border can be added to the top, right, bottom or left of the padding*/

/*Margin*/
/*Border can be added to the top, right, bottom or left of the border*/

/*Box Model: Size*/
/*The full size of a box is calculated by adding all of these properties*/
/* Content Area width + padding-left + padding-right + border-left + border-right + margin-left + margin-right*/

/*Applying the box model properties*/
/*It is possible to add every property individually*/
/*Padding*/
h2 {
    padding-top: 4px;
    padding-bottom: 8px;
    padding-right: 9px;
    padding-left: 3px;
}

/*We can also add these properties with a single line*/
h2 {
    padding: 4px 9px 8px 3px;
    /*top right bottom left*/
}
```
Web Forms
====================
```HTML
<!-- Web Forms -->
<!-- A Form is an element that allows a web page to get input from a user -->

<!-- Forms usually contain labels, inputs, text areas and submit buttons -->
<!-- In general, the processing of a form's information requires a back-end service -->

<!-- <form> tag-->
<!-- You can use it to create a form and add elements inside of it -->
<form>
    <!-- <label> tag-->
    <!-- Describes the type of information the user should enter-->
    <label>Form</label>
    <input type="text"/>
    <!-- <input type="submit"> tag -->
    <!-- Sends all the information from the form to the server -->
    <input type="submit" value="Submit"/>
</form>
<br/>

<!-- Form <input> types -->
<!-- The type attribute sets the type of input fields that will be displayed -->
<!-- These are common <input> types -->
<form>
    <input type="text"/>
    <input type="checkbox"/>
    <input type="radio"/>
    <input type="file"/>
    <input type="password"/>
    <input type="submit">
</form>
```
```CSS
/* Styling forms*/
/* labels and inputs are inline-level tags*/
/* In general, it is better to display one on top of the other like block-level tags*/
.styled-form label,input{
    display: block;
}
/*You can style the elements inside the form like any block-level tag*/
.styled-form label{
    margin-bottom: 10px;
}
.styled-form input{
    width: 500px;
    margin-bottom: 25px;
}

/* Attribute selectors */
/* A method to style a tag based on one of its attributes*/

/* Styling the submit button separately */
/* The submit button is an input tag so the previous input selector properties are affecting the way it is displayed */

/* In order to create this selector, you need: */
/* The name of the attribute and the value of the attribute */
.styled-form input[type=submit]{
    width: 120px;
    font-size: 30px;
}

/* Styling Inputs */
/* The container around an input is a border, so you can style it with the border property */
.styled-form input[type=text]{
    border: 2px solid #7facaa;
}
```

Run and Play
====================
All the html files are linked to their respective CSS files. Open your browser, change the content and start learning!

<img src="https://s3-us-west-2.amazonaws.com/testdrivenlearningbucket/learnImage.png"/>

Questions ?
====================
If you have any questions, please feel free to ask me:
[Martin Chavez Aguilar](mailto:martin.chavez@live.com)

Contributors
====================
* [Martin Chavez Aguilar](http://martinchavezaguilar.com/) - Wrote the project

Continue Learning
====================
<a name="README">[<img src="https://camo.githubusercontent.com/eb464a60a4a47f8b600aa71bfbc6aff3fe5c5392/68747470733a2f2f7261772e6769746875622e636f6d2f766f6f646f6f74696b69676f642f6c6f676f2e6a732f6d61737465722f6a732e706e67" width="50px" height="50px" />](https://github.com/MartinChavez/Learn-Javascript)</a>
<a name="README">[<img src="https://pbs.twimg.com/profile_images/2149314222/square.png" width="50px" height="50px" />](https://github.com/MartinChavez/AngularJs-Basics)</a>
<a name="README">[<img src="https://s3-us-west-2.amazonaws.com/testdrivenlearningbucket/angularadvanced.png" width="50px" height="50px" />](https://github.com/MartinChavez/AngularJS-Advanced-Topics)</a>
<a name="README">[<img src="https://s3-us-west-2.amazonaws.com/testdrivenlearningbucket/csharp7.png" width="50px" height="50px" />](https://github.com/MartinChavez/CSharp)</a>
<a name="README">[<img src="http://precision-software.com/wp-content/uploads/2014/04/jQurery.gif" width="50px" height="50px" />](https://github.com/MartinChavez/jQueryBasics)</a>
