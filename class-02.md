# HTML

  - Bold and Italic: <b> and <i>
  - Superscript & Subscript: <sup> and <sub>
  - Line Breaks: <br/>
  - Horizontal Rules: <hr/>
  - Strong and Emphasis: <strong> and <em>
  - Quotations: <blcokquote cite=""></blockquote> and <q></q>
  - Abbreviations and Acronyms: <abbr title = ""></abbr> AND <acronym title=""></acronym>
  - Citations and Definitions: <cite></cite>; <dfn></dfn>
  - Author details: <address><a href="mailto:heidihcao@gmail.com"></a></address>
  - Changes to Content: <del>worst</del><ins>best</ins>; <s></s>
  
  - Using external css: <link href="" type="text/css" rel="stylesheet"/>
  - Using internal css: <style type="text/css"></style>
  - INHERITANCE by child elements
  - CSS Selectors: 
    1. universal selector *{} APPLIES TO ALL ELEMENTS IN THE DOC
    1. type selector h1{} Matches element names
    1. class selector .note{} Matches an element whose class attribute
    1. ID selector: #introduction {} Matches an element whose id attribute
    1. Child selector: li>a {} Matches an element that is the direct child of another (targets any <a> elements that are children of an <li> element)
    1. Descendant selector: p a {} Matches an element that is a descendent of another specified element (not just a direct child)
    1. Adjacent sibling selector h1+p {} Mathces an element that is next sibling of another
    1. General sibling selector h1~p {} Matches an element that is a sibling of another, although does not have to be directly preceding element
  
 
 <hr/>

# JS
  - Arrays are special types of variables that store more than one piece of related information
  - Javascript distinguishes between numbers 0-9, strings/text, and Boolean values (true or false).
  - Creating an array: 
    1. var colors; colors = ['white', 'black', 'custom']
    1. var colors = new Array('white', 'black', 'custom');
  - === strictly equal to
  - !=== strictly does not equal to
  - if (score>50){ <br>
      document.write('You passed!');<br>
    } else {<br>
      document.write('Try again');<br>
    }
  - Constructing comparison operators: var HasPassed = score>= pass;
  - && logical and
  - || logical or
  - ! logical not
  - logial expressions are evaluated left to right. you might commit short-circuit evaluation (i.e. false && anything --> true; true || anything --> true)
  
 <hr/>

# Class Notes
  - Data Types: *null* - specifically and explicitly defined 'let username =null;'
  - *undefined* - a primative value that is assigned to varaibles when no other value is assigned - 'let username;'
  

>From the Duckett HTML book:
>Chapter 2: “Text” (pp.40-61)
>Chapter 10: Ch.10 “Introducing CSS” (pp.226-245)

>From the Duckett JS book:
>Chapter 2: “Basic JavaScript Instructions” (pp.53-84)
>Chapter 4: “Decisions and Loops” only up to the section on switch statements (pp.145-162)
