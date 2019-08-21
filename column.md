---
description: >-
  The Column is used to set the vertical positions or flow of the child
  components.
---

# Column

### Description

The Column component is used to display the components in a column. Other components placed inside this component appears vertically.

### Usage

1. Drag and drop the **Column** component to a page container.
2. Set the required attributes.
3. Optionally, drag and drop any other components inside the **Column** component.
4. Save and run the page.

### Example

1. Drag and drop a **Column** component.
2. Set the component attributes value of **`layout direction`** to _**start**_ and **`perpendicular direction`** to _**stretch**_.
3. Drag and drop a **List Item** component inside the **Row** component.
4. Save and run the page.
5. When the page is loaded, the list item appears vertically. The values set in step 2 specifies the direction in which the flex starts.

## Associated Attributes

* **`style`:** Accepts a string value that affects different properties of the Column such as height, width, and color, based on the values provided. For example: `background:orange:height:200px`.
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

* **`fxFlex`:** This property should be used on elements within a **`fxLayout`** container and identifies the resizing of that element within the **`flexbox`**container flow such as **`flex-grow`**_**,**_ **`flex basis`**_**,**_ **`flex-shrink`**_**,**_ and**`flex-grow`**.
* **`fxLayoutGap`:** This property specifies margin gaps on components within a `flexbox` container. It accepts integer value. For example: _**20px,**_ and _**5em.**_
* **`wrap`:** This property specifies whether the flexible items should wrap or not. 
* **`Layout Direction`:** This property specifies how you can horizontally align the sub-components. It provides a drop-down list with the following options:
  * center
  * start
  * end
  * space-around
  * space-between
* **`Perpendicular Direction`:** This property specifies how you can vertically align sub-components in the page. It provides a drop-down list with the following options:
  * None
  * Center
  * Start
  * End
  * Stretch
* **`fxShow`:** This directive allows you to dynamically show the element. Choose **`True`** to dynamically show the element. Else, choose **`False`**.
* **`fxHide`:** This directive allows you to dynamically hide the element. Choose **`True`** to dynamically hide the element. Else, choose **`False`**.

**Support**

* **Devices:** Android, iOS
* **Browsers:** Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

