---
description: >-
  The Expansion Title component is used to display the title for the expansion
  panel components. It can be used inside the Expansion Panel Header component
  or it can be used individually.
---

# Expansion Title

## Description

Expansion Title component is used to display title for the Expansion Panel content. Only the title will be displayed, and the other components will be displayed after clicking the title.

## Usage

1. Drag and drop the **Expansion Panel** component.
2. Inside the **Expansion Panel** component, drag and drop the **Expansion Header** component. And inside **Expansion Header** component drag and drop the **Expansion Title** component.
3. Double click the **Expansion Title** component to display the list of attributes that can be used with it.
4. Fill the attributes which are needed and save the page.

### Example

1. Drag and drop the **Expansion Panel** component.
2. Inside the **Expansion Panel** component, drag and drop the **Expansion Header** component. And inside **Expansion Header** component drag and drop the **Expansion Title** component. 
3. Click the **Expansion Title** component. Set **`title`** to _**This is expansion panel title.**_
4. Save and run the page.
5. When the page is loaded the title will be displayed. And when the title is clicked, the **Expansion Header** panel will be extended.

## Associated Attributes

* **`Expansion Title label:`**The display name of the component.
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

* **`title`:** Specifies the title that is to be displayed when the page is loaded. 

**Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

