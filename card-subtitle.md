# card-subtitle

### Overview

A card subtitle component can be used to give a subtitle to any block. It contains the text value. It is used below the title component.

### Usage

It can be used where we want to set the subtitle of any block. It can be used inside a card or with some components to give the subtitle.

#### How to use

1. Drag and drop the card-subtitle component.
2. It has three attributes style, class and subtitle.
3. **Provide the value of style and class, and a text for the subtitle attribute.**

#### Example

**Display a card with card-title subtitle and some block of text** 1. Drag and drop a card. 2. Drag and drop a card-title, a card-subtitle and a paragraph component inside the card. 3. Now provide the title = Big Data in card-title, in subtitle component provide the subtitle = Hadoop and in paragraph provide some information about Hadoop. 4. Save and Run. 5. A card with title as Big Data, Subtitle as Hadoop and below that block of text will be displayed.

#### Associated Attributes

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

* **Subtitle:** It accepts string. And here we can give the data whatever we want to set as subtitle.

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

