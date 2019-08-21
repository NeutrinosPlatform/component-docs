# card-header

## Overview

A card header is similar to card, in which there will be title, subtitle and image as a attribute, but it can not contain any component inside it. It can be used alone as well as it can put inside a card.

## Usage

A card header can be used where a block should be displayed with a image, a title, a subtitle. Multiple card header can be placed inside a card to display a page which contains items as title, a subtitle and a image.

### How to use

1. Drag and drop a card header component.
2. Fill the attribute such as title, subtitle and imgSrc attribute.
3. Provide the title and subtitle as some text.
4. Give the path of the image which will be loaded, so if the image wallpaper.jpg is in assets folder the path can be assets:\android\wallpaper.jpg.

### Example

1. Drag and drop a card header.
2. Provide the title= Agra, subtitle=Taj Mahal and for imgSrc give the path of the image as assets:\android\taj.jpg. If the image is in android folder under assets.
3. Save and Run.
4. A card with a title Agra, a subtitle Taj Mahal and a image will be displayed on the screen.
5. Like this multiple card header can be put inside a card.

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

* **Title:** It accepts string value and we can give the title what we want to set a title. The text will be displayed in bold property. 
* **Subtitle:** This attribute contains the subttile a, which will be displayed below the title attribute, and it will be normal text. 
* **imgSrc:** This attribute stores the path of the image stored in the system and it displays the images based on the path if present. Such as \(android\wallpaper.jpg\). So this display the image of name wallpaper that is in jpg format.
* **Alt:** This will be displayed instead of image when the imgSrc does not load the image because of some reason. It can be string such as image not available.    

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

