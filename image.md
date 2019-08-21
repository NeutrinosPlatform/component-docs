# Image

## Overview

Image component is used to insert an image into a page.

## Usage

Used to display an image in a page. 

**Note:** Images are not technically inserted into the page, images are linked to HTML pages. The image component creates a holding space for the referenced image.

### How to use

1. Drag and drop the **Image** component. 
2. Double click the component to display the list of attributes that can be used with it.
3. Place the images inside the Assets editor and save the image inside one of the folders. Give the path of the image in the `imgsrc` attribute.
4. Fill the  required attributes.
5. Save and run the page.

### Example

1. Drag and drop the **Image** component. 
2. Double click the component to display the list of attributes
3. Input the component field\(s\) with the attribute value\(s\):  

    **`imgsrc`** _**= /&lt;path&gt;/neutrinos.png**_  

    **`Alt`**  = _**Neutrinos**_

4. Save and run the page.
5. When the page is loaded, the image will be displayed. If the image cannot be displayed a n alternate message **Neutrinos** will be displayed.

### Associated Attributes

* **Style:** It accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **Class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names which are defined as shown below:

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

* **`Assets src`**: Stores the source path of the image. It displays the image if the image is present in the path that is specified. For example: _**android\wallpaper.jpg**_ ****displays the image which is in **.jpg** format. 
* **`[src]`**: The source location of the image.
* **`Secure URL`**: The Secure URL of the image.  If you do not use a secure URL, app users may get warnings that the app contains insecure data.
* **`[collection name]`**: The name of a collection which contains images that can be switched depending on a condition.
* **`[image filter]`**:  Allows you to apply filters to the image.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

