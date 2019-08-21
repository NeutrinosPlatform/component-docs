# card-content

## Overview

A card content is a container in which a paragraph or text can be put inside. It is basically intended for block of text but it can contain other components also such as card-title, card-subtitle, card-image etc.

## Usage

It is a container of blocks that can contain text, and it can also store buttons, card-title, card-subtitle, card-image etc.

### How to use

1. Drag and drop a card content it has attributes like style and class. 
2. In this card-content other components can be rendered and they can be displayed in a block.

### Example

**A card-content with a title and paragraph**  
1. Drag and drop a card-content and fill the attributes such as style and class. 2. Drag a card title and place it inside card content and set the title=Dog breed. 3. Drag and drop a paragraph component inside a card content below the card title and provide the text as information. 4. Save and Run. 5. A block with the title as Dog breed and the paragraph will be displayed.

## Associated Attributes

* **Style:** It accepts a string value and affects the different properties \(height, width, color etc.\) of the component based on the values provided \(eg. background:orange;height:200px;\).
* **Class:** "Class" attribute is used to point to a class in a style sheet. A class contains one or more style statements. Classes are created inside the "Style" tab which is opened by selecting the "Style" side menu. The "Class" attribute accepts space separated class names \(eg. class1, class2\) which are defined in the "Style" tab as shown below.

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

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

