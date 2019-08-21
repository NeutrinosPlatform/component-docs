---
description: >-
  Expansion Panel is a container which contains some of the components such as
  expansion header, expansion title, and expansion description.
---

# Expansion Panel

## Description

Expansion Panel component can be used where the data to be displayed in a expanded view, and will be shown and hidden depending on what you set in the **`onclick`** event. By default, only the title and description will be shown and other components will be hidden. They will displayed when the user clicks on it. 

Expansion Panel can be used along with all these component or it can be put inside a expansion panel outlet component.

## Usage

1. Drag and drop an **Expansion Panel** component.
2. Fill the required attributes.
3. Place other expansion components within the component.
4. Save and run the page.

### Example

1. Drag and drop an **Expansion Panel Outlet** component, and inside that drag and drop an **Expansion Panel** component.
2. Drag and drop an **Expansion Header** component inside **Expansion Panel**.
3. Drag and drop **Expansion Title** and **Expansion Description** component inside the expansion header component.
4. Click on **Expansion Title** and set the **`Expansion Title Label`** as _**Personal Detail**_ . Click the **Expansion Description** component and provide the **`Expansion Description label`** as _**enter your name**_.
5. Save and run the page.
6. An **Expansion Panel** will be displayed with the title as _**Personal Detail**_ and description as _**enter your name**_. Other palette components can be inserted inside the panel according to your app requirements.

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

* **`*ngFor`:** Used when there are multiple expanded panel components to iterate through an array of objects of the expanded panel and display them. The array of objects are defined in  the `.ts` file. 
* **`(opened)`:** This attribute contains an event that should be emitted every time the Accordion Item is opened, so a method or function will be defined and it will be called. Inside the function, actions will be defined as to what should happen when the item is open.
* **`(closed)`:** This attribute contains an event that should be emitted every time the Accordion Item is closed, so a method or function will be defined and it will be called. Inside the function, actions will be defined as to what should happen when the item is closed.
* **`Hide Toggle`:** Used to check whether the expansion indicator should be hidden. You can set the value to True or False. 
* **`[expanded])`:**Accepts any type of values, to check whether the accordion Item is expanded.
* **`(afterCollapse)`**: Used to specify the event emitted after the body's collapse animation happens.
* **`(afterExpand)`**: Used to specify the event emitted after the body's expansion animation happens.

**Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +  

