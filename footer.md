---
description: >-
  A Footer component defines a footer for a document or section. It is used when
  the content should be displayed at the bottom of the page.
---

# Footer

## Description

A Footer component typically contains author information, copyright information, contact information, sitemap, back to top links, and related documents. There can be several footer components in one document.

## Usage

1. Drag and drop a **Footer** component.
2. Fill the attributes. 
3. Optionally, add other components.
4. Save and run the page.

### Example

**Display a Footer with Neutrinos copyright information.**

1. Drag and drop a **Footer** component to your page.
2. Drag and drop a **HTML5** component inside the Footer component.
3. Open the HTML5 component's attribute window and select **Paragraph** in the Element Type drop-down list. 
4. Click the HTML5 editor on your page, an editor block is displayed in the bottom of the screen. Enter this code in the editor: **`<p>`**_**© Neutrinos. All rights reserved**_.**`</p>`**. 
5. Drag and drop a **Image** component inside the **Footer** component.Double click the component to display the list of attributes.
6. Input the Image attribute fields with the following attribute values:  

    **`imgsrc`** _**= /&lt;path&gt;/neutrinos.png**_  

    **`Alt`**  = _**Neutrinos Logo**_

7. Save and run the page. You will see a footer displayed on the page with the copyright information and Neutrinos logo.

## **Associated Attributes**

* **`Footer label:`** Display name of the footer.
* **`style`:** Accepts a string value that affects different properties of the component such as height, width, and color, based on the values provided. For example: `background:orange:height:200px`.
* **`class`:** Used to point to a class in a style sheet.  Each class contains one or more style statements defined in the **Style** editor. The `Class` field accepts space separated class names such as `class1 class2` , where each class is defined in the Style editor as shown below:

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

