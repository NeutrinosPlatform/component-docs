---
description: >-
  The Expansion Description component is used for describing the expansion panel
  components.
---

# Expansion Description

## Description

The Expansion Description component can be used inside the Expansion Panel Header component or it can be used individually to display the description.

## Usage

1. Drag and drop the **Expansion Panel** component.
2. Inside the **Expansion Panel** component, drag and drop the **Expansion Header** component. And inside **Expansion Header** component drag and drop the **Expansion Description** component.
3. Double click the **Expansion Description** component to display the list of attributes that can be used with it.
4. Fill the attributes which are needed and save the page.

### Example

1. Drag and drop an **Expansion Description** Panel into a page container. Click the component. Enter _**This is a description panel**_ in the **Expansion Description Label** field.
2. Save the page and run.
3. When the page is loaded, the attribute description will be displayed. And when the description is clicked, the **Expansion Header Panel** will be extended.

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

* **`Expansion Description label:`**The display name of the component.
* **`description`:** Used to give description for the expansion panel. 

**Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

