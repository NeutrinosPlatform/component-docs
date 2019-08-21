---
description: A List component contains List Item components in the form of line items.
---

# List

## Description

List component contains a number of List Item components.There is no requirement to set the number of columns. It is an unordered list, and the list items will come one below the other.

## Usage

1. Drag and drop a **List** component.
2. Set the attribute such as style and class. 
3. Insert one or more **List Items** component inside the **List** component.

### Example

**Display a list of three items:**

1. Drag and drop a **List** component and set the attribute such as **`style`** and **`class`**.
2. Drag and drop a **List Item** component inside the **List** component,  and set the attributes of the **List Item** component_._ 
3. **`ngFor`** is used to iterate through the object and access the items of the objects, if **folders** is an object which has attribute as **name\(name of folder\)** as a string type, with three items in the folder object, set the field in **`ngFor`** as let folder of folders. 
4. **`Label`** attribute displays the name as list items, provide the name as **`folder.name`**, this will access the folders object and get the **name** value. If the folders object contains three values such as photos, work and document, then the list items will be photos, work and document. 
5. Save and run the page. A list with three items will be displayed.

## Associated Attributes

* **`List label:`**Used to put a display text on the component describing what purpose it has for the user.
* **`style`:** Accepts a string value that affects different properties of the List such as height, width, and color, based on the values provided. For example: `background:orange:height:200px`.
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

