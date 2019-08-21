# flex-layout-row

## Overview

Flex-layout-row is used to set the positions or flow of the child components horizontally. It has following properties like style, Class, fxFlex, fxLyoutWrap, fxLayoutgap, Fxlayoutalign, fxShow, and fxHide.  
**Note:** By default some of the attributes will be set to default values. Change it according to the need.

## Usage

Flex-layout-row is used to display the components in a row. Components placed inside flex-layout-row appears horizontally.

### How to use

1. Drag and drop the flex-layout-row component.
2. Fill the required attributes. 
3. After that drag and drop any other components inside the flex-layout-row component.

### Example

1. Drag and drop a flexlayoutrow component.
2. Set the component attributes value with “layout direction = start” and perpendicular “direction = start”.
3. Drag and drop some other components like button and textbox inside the flexlayoutrow component.
4. Save it and run.
5. When the page is loaded the components button and textbox appears horizontally. And the value “layout direction = start” and perpendicular “direction = start” specifies the direction in which the flex starts.

## Associated Attributes

* **Style:** It accepts a string value and affects the different properties \(height, width, color etc.\) of the component based on the values provided \(eg. background:orange;height:200px;\).
* **Class:** "Class" attribute is used to point to a class in a style sheet. A class contains one or more style statements. Classes are created inside the "Style" tab which is opened by selecting the "Style" side menu. The "Class" attribute accepts space separated class names \(eg. class1 class2\) which are defined in the "Style" tab as shown below.

  ```css
    .class1 {
        border-radius:10px;
        flex-basis:10%;
        height:100px;
    }
    .class2 {
        border-radius:10px;
        flex-basis:10%;
        height:100px;
    }
  ```

* **fxFlex:** This property should be used on elements within a fxLayout container and identifies the resizing of that element within the flexbox container flow such as flex-grow, flex basis, flex-shrink,flex-grow.
* **wrap:** This property specifies whether the flexible items should wrap or not. It has values such as nowrap, wrap, wrap-reverse, initial,inherit.
* **fxLayoutGap:** This can be used to specify margin gaps on children within a flexbox container. It accepts integer value. Such as 20px, 5em etc.
* **Layout Direction:** This can be used to specify how the children components of this component should be aligned horizontally. It accepts string values such as center, start, end etc.
* **Perpendicular  Direction:** This can be used to specify how the children components should be aligned vertically. It accepts string values such as center, start, end etc.
* **fxShow:** This directive allows developers to dynamically show the element. It accepts boolean values such as true or false.
* **fxHide:** This directive allows developers to dynamically hide the element. It accepts boolean values such as true or false.

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

