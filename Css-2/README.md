# CSS Interview questions 👋

### 1. how to add comments on css ?

```bash
  =>  /* This is a single-line comment */
  =>  /* This is
      a multi-line
      comment */
```
### 2. Why do we use pseudo-class ?

```bash

=> A pseudo-class is used to define a special state of an element.

    For example, it can be used to:

        * Style an element when a user mouses over it
        * Style visited and unvisited links differently
        * Style an element when it gets focus

    /* unvisited link */

    a:link {
    color: red;
    }

    /* visited link */

    a:visited {
    color: green;
    }

    /* mouse over link */

    a:hover {
    color: hotpink;
    }

    /* selected link */

    a:active {
    color: blue;
    }
```
### 3. How is specificity applied ?

```bash
    => If there are two or more CSS rules that point to the same element, the selector with the highest specificity value will "win", and its style declaration will be applied to that HTML element.

    => "Every CSS selector has its place in the specificity hierarchy"
    * There are four categories which define the specificity level of a selector:


    * Inline styles - Example: <h1 style="color: pink;">
    * IDs - Example: #navbar
    * Classes, pseudo-classes, attribute selectors - Example: .test, :hover, [href]
    * Elements and pseudo-elements - Example: h1, :before

    "Note" => There is one exception to this rule: if you use the !important rule, it will even override inline styles!

    * Inline style gets a specificity value of 1000, and is always given the highest priority!
    * add 100 for each ID value,
    * add 10 for each class value (or pseudo-class or attribute selector),
    * add 1 for each element selector or pseudo-element.
```
### 4. What method allows an element to be moved from its current position ?

```bash
=> The positioning of an element can be done using the top, right, bottom, and left properties. These specify the distance of an HTML element from the edge of the viewport. To set the position by these four properties, we have to declare the positioning method.
```
### 5. what properties does flex model have ?

```bash
=> The flex CSS shorthand property is the combination of flex-grow, flex-shrink, and flex-basis property. It is used to set the length of flexible items. The flex property is much responsive and mobile-friendly. It is easy to position child elements and the main container.
```
### 6. What is the difference between flex and grids ?

```bash
=> Grid is made for two-dimensional layout while Flexbox is for one. 
=> This means Flexbox can work on either row or columns at a time, but Grids can work on both.
```
### 7. Give an example where we have to use grids and where you have to use flexbox ?

```bash
=> If you are using flexbox and find yourself disabling some of the flexibility, you probably need to use CSS Grid Layout. An example would be if you are setting a percentage width on a flex item to make it line up with other items in a row above. In that case, a grid is likely to be a better choice.
```
### 8. Give an example where you cannot use flexbox, and you can only use grids ?

```bash
=> when you have to manage two dimension at a time .
```
### 9. What are combinators? give examples of how you can use them ?

```bash
    Answer ...
```
### 10. What does object-fit do ?

```bash
    Answer ...
```
### 11. What does rotate do ?

```bash
    Answer ...
```
### 12. What rule can be used to define animations ?

```bash
    Answer ...
```
### 13. When working with attribute selectors, how can you select elements which contain a particular attribute value ?

```bash
    Answer ...
```
### 14. What does @media do ?

```bash
=> The @media rule is used in media queries to apply different styles for different media
```
### 15. What can be used to override properties of an element ?

```bash
1. By increasing there specificity .
2. use !important .
```
### 16. How can you select every alternate elements in a list of elements using css ?

```bash
=> :nth-child(even);
```
### 17. What is the ranking of selectors with respect to specificity ?

```bash
    => "Every CSS selector has its place in the specificity hierarchy"
    * There are four categories which define the specificity level of a selector:


    * Inline styles - Example: <h1 style="color: pink;">
    * IDs - Example: #navbar
    * Classes, pseudo-classes, attribute selectors - Example: .test, :hover, [href]
    * Elements and pseudo-elements - Example: h1, :before

    "Note" => There is one exception to this rule: if you use the !important rule, it will even override inline styles!

    * Inline style gets a specificity value of 1000, and is always given the highest priority!
    * add 100 for each ID value,
    * add 10 for each class value (or pseudo-class or attribute selector),
    * add 1 for each element selector or pseudo-element.
```
### 18. how can we apply same styles to multiple selectors ?

```bash
1. By giving same class , or Id .
2. * tr:nth-child(even) {background: #CCC}
   * tr:nth-child(odd) {background: #FFF}
```
### 19. What are the differences between relative and absolute in CSS ?

```bash
=> The position CSS property sets how an element is positioned in a document. The top, right, bottom, and left properties determine the final location of positioned elements.

relative
The element is positioned according to the normal flow of the document, and then offset relative to itself based on the values of top, right, bottom, and left. The offset does not affect the position of any other elements; thus, the space given for the element in the page layout is the same as if position were static.

This value creates a new stacking context when the value of z-index is not auto. Its effect on table-*-group, table-row, table-column, table-cell, and table-caption elements is undefined.

absolute
The element is removed from the normal document flow, and no space is created for the element in the page layout. It is positioned relative to its closest positioned ancestor, if any; otherwise, it is placed relative to the initial containing block. Its final position is determined by the values of top, right, bottom, and left.

This value creates a new stacking context when the value of z-index is not auto. The margins of absolutely positioned boxes do not collapse with other margins.

=> position: relative places an element relative to its current position without changing the layout around it,
 whereas 
=>position: absolute places an element relative to its parent's position and changing the layout around it.
```