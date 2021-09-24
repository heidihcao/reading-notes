
# JS: an interpreted programming language
- **script**: a series of instructions that the computer can follow in order to achieve a goal. 
    1. flowchart: tasks; generic step, event, input or output, decision (see pic on page 23)
    1. lists: steps required

- **objects and properties**: make, currentSpeed, color, fuel
- **events**:brake, happens where: driver slows down
- **methods**: represent things people need to do with objects. <br> They can retrieve/update the values of an object's properties, i.e. changeSpeed(), makeBooking()

- *How a browswer sees a webpage*:
    1. browser receives an HTMl page
    2. creates a model of the page and stores it in memory
    3. use a rendering engine to show the page on the screen
- All major browser use a JavaScript interpreter to translate JavaScript instructions into ones the computer can follow

- *How HTML, CSS, and JavaScript fit*:
    1. <html> CONTENT LAYER
    1. {css} PRESENTATION LAYER
    1. javascript() BEHAVIOR LAYER
    
- document.write('Good Afternoon');
- JS runs where it is found in HTML: when the browser comes across a <script> element;
    <script src=".js"></script>


## HTML 
Tag: <element></element>
<!DOCTYPE html> Opening in HTML
<! ----> to **comment** in HTML

**ID attribute**: <p id="pullquote"></p>

**Class attribute**:<p class="important"></p>

Block elements:<ul> <li></li></ul>
Inline statements: <em></em><b></b>

**Grouping text and elements inline**
- <span class="gallery">
    </span>
    
**Grouping text and elements in a block OR sectioning elements**
- <div id="header">
    </div><! --end of header -->
    
**Iframes cut windows into your pages through which other pages can be displayed**
<iframe
        width=""
        height=""
        src="">
</iframe>

**Figure**
<figure>
    <img src=""/>
    <figcaption> SOMETHING </figcaption>
</figure>


**Info about your page**
<meta name=""
      content="">
    
**Others*
<nav></nav>
<article></article>
<section></section>
<hgroup></hgroup>
<aside></aside>: when used inside <article> element, contain info that is related to the article; outside <article>, acts as a container for content related to the entire page
<a href=""></a>: place around a block level element that contains child elements. This allos you to turn an entire block into a link   
    

>From the Duckett HTML book:
>Introduction (pp.2-11)
>HTML Chapter 1: “Structure” (pp.12-39)
>HTML Chapter 8: “Extra Markup” (p.176-199)
>HTML Chapter 17: “HTML5 Layout” (pp.428-451)
>HTML Chapter 18: “Process & Design” (pp.452-475)

>From the Duckett JS book:
>Introduction
>JS Chapter 1: “The ABC of Programming” (pp.11-52)
