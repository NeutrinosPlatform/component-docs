---
description: >-
  A Header element typically contains one or more header elements, logo or icon,
  author information. There can be several Header components in one document.
---

# Header

## Description

A Header component is used when the content is to be displayed with some special properties. For example, when you want to use a  bigger font size, or when you want to display the text in bold. 

Various components can be inserted inside a header component. 

### How to use

1. Drag and drop a **Header** component.
2. Fill the attributes. 
3. Optionally, add other components.
4. Save and run the page.

### Example

**Display a header component with a title, a subtitle in and a paragraph component** 

1. Drag and Drop a **Form** component  into the page.
2. Drag and drop a **Header** component inside the **Form** component.
3. Drag and drop a **Image** component inside the **Header** component.Double click the component to display the list of attributes.
4. Input the Image attribute fields with the following attribute values:  

    **`imgsrc`** _**= /&lt;path&gt;/neutrinos.png**_  

    **`Alt`**  = _**Neutrinos Logo**_

5. Save and run the page.
6. When the page is loaded, the Neutrinos logo will be displayed inside the header component. 

## Associated Attributes

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

