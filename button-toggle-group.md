# button-toggle-group

## Overview

Button toggle group contains many buttons whose behavior is similar to radio buttons. Only one of the buttons can be selected at a time.

## Usage

Selecting any one of the unselected buttons in a button group will unselect the previously selected button and selects that button.

### How to use

1. Drag and drop the “Button Toggle Group” component from “Forms Control” Category where it is needed in that page.
2. Double click on the component and give values to the attributes.

### Example

1. Create a page called “page”.
2. Drag and drop the “Button Toggle Group” component.
3. Double click on that component.
4. In the “Ts” file, create a property called “buttons” and set its value as below.

   ```typescript
    buttons = [{"value":"Bold"}, {"value":"italic"}, {"value":"strike"}];
   ```

5. Set the value of \[toggleOptions\] to “buttons”.
6. Write a function in Ts file as below:

   ```typescript
   onValueChange(){
       console.log("val changed")
   }
   ```

7. Set the \(valueChanged\) attribute to “onValueChange\(\)”.
8. Set "\[disableIndex\]" to “0”.
9. Save the changes.
10. Open the address where the app is running, and try selecting a button from the button group.
11. The console will output “val changed”. 

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

* **\[align\]:** Sets the alignment of the buttons in button group. Takes 'vertical' or 'Horizontal' as its value \(with single quotes\).
* **\[disableIndex\]:** Index of the button that should be disabled by default. Takes a number as its value.
* **\[checkIndex\]:**  Index of the button that should be selected by default. Takes a number as its value.
* **\(valueChange\):** Takes function\( that is defined in the "Ts" file\) name as an argument which will be called whenever the value of button group changes. eg. onValChange\(\)
* **\(indexChange\):**  Takes function\( that is defined in the "Ts" file\) name as an argument which will be called whenever different button gets selected in button group. eg. onIndexChange\(\)

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

