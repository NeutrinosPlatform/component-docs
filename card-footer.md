# card-footer

## Overview

A card footer is a sub-container of card. In this we can give the information which will be displayed as a footer in the card.

## Usage

Card footer component can be used where the data should be displayed as footer, at the bottom of any container. It can contain data such as string value, logo or anything inside it.

### How to use

1. Drag and drop a card footer component where it can be used.
2. Fill the attribute such as style and class.
3. It can be used within pages which require a footer.
4. Put other components inside the footer component which can be displayed as a footer.

### Example

**Display a card with a title, a image, a paragraph about that image and a card footer** 1. Drag and drop a card component and provide the style and class values. 2. Drag and drop a card title inside the card and give the title=Taj Mahal. 3. Drag and drop a paragraph inside the card component below the card-title and provide the path of the image in imgSrc attribute that is stored in the system so if the image is in asset folder then the path can be \(asset\android\taj.jpg\) and, the image taj.jpg will be displayed on the screen. 4. Now, drag and drop a paragraph component inside the card, below the card-image, provide an image description in text attribute. 5. Now drag and drop a card footer inside the card below all components and drag a paragraph component inside the footer component and provide some text that can be displayed as a footer on the screen.  
6. Drag and drop a card component and provide the style and class values. 7. Drag and drop a card title inside the card and give the title = Tajmahal. 8. Drag and drop a paragraph inside the card component below the card-title and provide the path of the image in imgSrc attribute that is stored in the system so if the image is in asset folder then the path can be \(asset\android\taj.jpg\) and, the image taj.jpg will be displayed on the screen. 9. Now, drag and drop a paragraph component inside card below the card-image and in text attribute provide some information about the image. 10. Now, drag and drop a card footer inside the card below all components and drag a paragraph component inside the footer component and provide some text that can be displayed as a footer on the screen.

## Associated Attributes

* **Style:** It accepts a string value and affects various properties such as height, width, color etc. of the component based on the values provided \(eg. background:orange;height:200px;\).
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

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

