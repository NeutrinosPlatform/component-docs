# card-title

## Overview

A card title can be used to give a title to any block. It contains the text value.

## Usage

It can be used where we want to set the title of any component. It can be used inside a card or with some components to give the title.

### How to use

1. Drag and drop the card-title component.
2. It has three attributes style, class and title.
3. Provide the value of style and class, and in title attribute give the title that will be set as title.

### Example

**Display a card with card-title and some block of text.** 1. Drag and drop a card. 2. Drag and drop a card-title and a paragraph component inside the card. 3. Now provide the title=Big Data and in paragraph provide some information about Big Data. 4. Save and Run. 5. A card with title as Big Data and below that block of text will be displayed.

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

* **Title:** It accepts string value and we can give the title what we want to set as title. The text will be displayed in bold property. 

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

