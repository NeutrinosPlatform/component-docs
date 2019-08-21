---
description: Expansion Header is used to show a summary of the panel content.
---

# Expansion Header

## Description

The Expansion Header shows a summary of the panel content and acts as the control for expanding and collapsing. This header may optionally contain Expansion Title and Expansion Description components. By default, the Expansion Header includes a toggle icon at the end of the header to indicate the expansion state. This icon can be hidden via the **`hideToggle`** property.

## Usage

1. Drag and drop an **Expansion Panel** component.
2. Drag and drop an Expansion Header component inside the **Expansion Panel** component.
3. Fill the required attributes.
4. Place other expansion components within the component.
5. Save and run the page.

### Example

1. Drag and drop an **Expansion Panel** component.
2. Inside the **Expansion Panel** component, drag and drop the **Expansion Header** component.
3. Double click the **Expansion Header** component. Input the component field with the following attribute values:  

   **`collapsedheight`** = _**50**_  

   **`expandedheight`** =  _**50**_

4. Save the page and run.
5. The header will be loaded with the specified height when collapsed and expanded.

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

* **`collapsedheight`:** Specifies the height of the header while the panel is collapsed. 
* **`expandedheight`:** Specifies the height of the header while the panel is expanded.

**Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

