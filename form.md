---
description: >-
  A Form component can be used whenever there is a requirement for data entry.
  It can be used to enter, edit, or display data from a configured data source.
---

# Form

## Description

A Form component is a container which contains several other components such as Input, Radio button, Checkbox, Buttons etc. Users interacts with all the components inside a form  component and can change their value  at run time.

## Usage

1. Drag and drop a **Form** component.
2. Set the **`style`** and **`class`** attributes.
3. Drag and drop other components inside the **Form** component.

### Example

**Display a login page:**

1. Drag and drop a **Form** component into the page. 
2. Drag and drop a **HTML5** component inside the form and set the Element type as **Paragraph**. Open the HTML editor and set the text as _**Username**_. 
3. Drag and drop a **Input** component into the form to accept username.
4. Drag and drop another **HTML** 5 component, set the Element type as **Paragraph**, and set the text as _**Password**_. 
5. Drag and drop an **Input** component to accept user password. 
6. Drag and drop a **Button** component below the Input component and name the button as _**Submit**_. Set the **`onClick`** attribute of the button to accept user input.
7. Save and Run the page.
8. On rendering, you will see a login page which accepts **Username** and **Password** fields and the **Submit** button.

## **Associated Attributes**

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

* **action:** Describes where to send the data when the form is submitted. Example- landing page.
* **method:** Specify the method to change a control's value programmatically.
* **target:**  Specify where to display the response that is received after submitting the form.
* **\(onsubmit\):** The function to be executed when a form is submitted.
* **\(onreset\):** The function to be executed when the form is reset.

**Support**

* **Devices:** Android, iOS
* **Support**
* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

