---
description: >-
  An Expansion Panel Outlet component is a container which provides the
  expandable view, where some of the content will be hidden and will be
  displayed when the user clicks on the component.
---

# Expansion Panel Outlet

## Description

An Expansion Panel Outlet component can be used where the data is to be displayed in a expanded view on click. By default, only the title and description of the component is displayed, and other components will displayed when the user clicks on it.

## Usage

1. Drag and drop a **Expansion Panel Outlet** component.
2. Fill the required attributes.
3. Drag and drop other components inside it according to your app requirements.
4. Save and run the page.

### Example

1. Drag and drop an **Expansion Panel Outlet** component. Inside it, drag and drop a **Expansion Panel** component.
2. Drag and drop a **Expansion Header** component inside the expansion panel.
3. Drag and drop **Expansion Title** and **Expansion Description** components inside the **Expansion Header** component.
4. Click on the **Expansion Title** component. Set **`Expansion Title Label`** = _**Personal Detail**_ . Click the **Expansion Description** component and provide the description attribute as _**enter your name**_.
5. Save and run the page.
6. An **Expansion Panel** will be displayed with the title as _**Personal Detail**_ and description as _**enter your name**_. Many other components can be inserted inside each of these components according to your app requirement.

## Associated Attributes

* **`style`:** Accepts a string value that affects different properties of the Card such as height, width, and color, based on the values provided. For example: `background:orange:height:200px`.
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

* **`[displayMode]`:** Used for all expansion panels in the accordion. You can set the mode to:  
  * `default`: A gutter-like spacing is placed around any expanded panel, placing the expanded panel at a different elevation from the rest of the accordion. 
  * `flat`: No spacing is placed around expanded panels, showing all panels at the same elevation.
* **`Multiple Expansion`:**  A Boolean value to indicate **`True`** or **`False`**. Depending on the Boolean value you set, the component checks whether the accordion should allow multiple expanded accordion items simultaneously or not.

  \*\*\*\*

**Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

