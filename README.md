<a name="README"><img src="http://static1.squarespace.com/static/54b6c223e4b0ad6fb5d5569b/t/54bec5a4e4b0c74e7f3b09e9/1421788582011/large_html.jpg" width="300px" height="200px"/></a>

# HTML5/CSS3: Advanced Topics

Use this tutorial as a guide to learn HTML5 and CSS3. Each unit contains an annotated lesson that can assist you in developing your Web Development skills.

Topics
================
- HTML5: Overview
- Transform: Translate
- Transform: Rotate
- Transform: Scale
- Transform: Skew
- Transition

Suggested prerequisites
====================
<a name="README">[<img src="http://static1.squarespace.com/static/54b6c223e4b0ad6fb5d5569b/t/54bec5a4e4b0c74e7f3b09e9/1421788582011/large_html.jpg" width="65px" height="50px" />](https://github.com/MartinChavez/HTML-CSS)</a> 

HTML5: Overview
====================
```HTML
<!-- HTML5 -->
<!-- HTML5 is the definition used to refer to the latest version of HTML -->
<!--
 Features:
* New HTML elements and attributes
* CSS3 support
* Video and audio elements
* 2D and 3D graphics
* Local storage
* Local SQL database
-->

<!-- In HTML5, there is only one simple DOCTYPE, it has the following syntax -->
<!DOCTYPE html>

<html lang="en">
<head>
    <!-- In HTML5, you can specify the encoding by simply adding the charset attribute -->
    <meta charset="UTF-8">

    <!-- You don't need to specify the type attribute anymore (for <script> and <link>) -->
    <!-- A modern browser will infer that the file is javascript or css  -->
    <script src=""></script>
    <link rel="stylesheet" href="css/overview.css"/>

    <title>HTML/CSS: Overview</title>
</head>
<body>
<h1>HTML5: Overview</h1>

<h1>Tag Updates</h1>
<!-- Tag Updates -->
<!-- <i> tag represents text in a different "tone", like a thought -->
<p>This <i>text</i> has the i tag </p>
<!-- <b> tag represents stylistically offset text  -->
<p>This <b>text</b> has the b tag </p>
<!-- <em> tag represents "stress" emphasis -->
<p>This <em>text</em> has the em tag </p>
<!-- <strong> tag represents strong importance -->
<p>This <strong>text</strong> has the strong tag </p>
```
Animations
====================
```CSS
/* CSS3: Animations */

/* Transforms */
/*
- This property allows you to translate, rotate, scale, and skew elements in CSS
*/

/* Translate */
/*
- The translate() method moves an element from its current position
  (according to the parameters given for the X-axis and the Y-axis).
*/
.transform{
    /* Translate the element 20px to the right */
    /* Translate the element 30px to the down */
    transform: translate(20px, 30px);
    /* Translate parameters*/
    /*
    - A translation value for the x-axis, which can be either a length or a percentage
    - A translation value for the y-axis, which can be either a length or  a percentage, if not specified,the value is 0
    */
}
/* It is possible to use TranslateX and translateY to translate the x and y values individually */
.transform {
    transform: translateX(30px);
}
.transform {
    transform: translateY(40px);
}

/* Rotate */
/*
-  It is possible to rotate an element clockwise around its origin by the specified angle
*/
.rotate {
    transform: rotate(45deg);
}

/* Scale */
/*
- You can do a 2D scale by a specified unitless number
*/
.scale {
    /* The element is scaled to the unitless number: 4 */
    /* If you don't specify a value for y-axis, it defaults to the value of x-axis */
    transform: scale(4, 1);
}

/* Skew */
/*
- An element is skewed around the x or y axis by the angle specified
- You can use skewX and skewY that take an angle as parameters
*/
.skew{
    transform: skewX(-25deg);
    transform: skewY(25deg);
}

/* Transitions */
/*
- Allow you to transition between two states of a specified element
*/
.transition{
    /* Parameters (in order):
    - Property: The CSS property you want to transition
    - Duration: The amount of time you want the transition to take place
    - Timing function: Timing of the transition itself (ease, ease-in, ease-in-out, linear, etc)
    - Delay: The amount of time to wait between the change that is being requested on a specific property,
      and the start of the transition
    */
    /* The background-color transitions from grey to crimson over the period of .5s*/
    transition: background-color 0.5s ease-in-out;
}
.transition:hover{
    background-color: crimson;
}

.transition:hover{
    color: navajowhite;
}
/* Using 'all' as the transition-property, we can transition multiple properties at once */
.transition{
    transition: all 0.5s ease-in-out;
}

/* Progressive Enhancement */
/*
- Refers to the use of newer features that add to the experience in modern browsers that support those features,
  but doesn't detract from the experience in older browsers.
*/
.progressive-enhancement{
    background: #ccc;
    /* If the border-radius and box-shadow properties aren't supported, we still get a usable experience */
    border-radius: 10px;
    box-shadow: 0 1px 1px rgba(0,0,0,0.75);
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
