# card-image

## Overview

A card image component contains an image, a card image can be used alone or with a card.

## Usage

We can use card image where we want to display an images. Put the image inside this component and the image will be displayed.

### How to use

1. Drag and drop a card-image.
2. Fill the properties such as style, class imgSrc and alt.
3. In imgSrc provide the path of the image which should be available in the assests folder.

### Example

1. Drag and drop a card component.
2. Drag a card-title component and place it inside the card and set the title as Dog.
3. Drag and drop a card-image component inside a card, below the card title component. And fill the properties such as style, class, in imgSrc set the path of the image which is stored in the system. Such as \(assets:\android\dogimage.jpg\) and in alt attribute, set some text that will be displayed when the image will not load. Such as alt="image not available".
4. Save and Run.
5. A card with an title Dog and a dog image will be displayed.

## Associated Attributes

* **Style:** It accepts a string value and affects properties such as height, width, color etc., of the component based on the values provided \(eg. background:orange;height:200px;\).
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

* **imgSrc:** this property stores the path of the image stored in the system and it displays the image based on the path if present. Such as \(android\wallpaper.jpg\). So this displays the image which is in jpg format.
* **Alt:** this will be displayed instead of image when the imgSrc does not load the image because of some reason. It can be string such as\("image not available"\). 

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

