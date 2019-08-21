---
description: >-
  A Step component is used to create a page that is divided into various steps.
  It can be displayed horizontally or vertically.
---

# Step

### Description

A step component is used inside a Stepper component. A Step component can contain different components such as Textbox, Buttons, Radio buttons, images,etc. 

## Usage

1. Drag and drop a stepper component.
2. Fill the required properties.
3. Drag and drop a Step component inside the Stepper component.

### Example:

**Create a stepper with login process.**

1. Drag and drop a **Stepper** component. 
2. In the Attributes window,  enter _**matHorizontalStepper**_ for the **`matHorizontalStepper`** ``option. 
3. If there are three **Step** components, labeled as **`getUsername`**, **`getPassword`**, and **`submit`**, drag and drop these three step components inside the **Stepper** component, and give the label as _**getUsername**_, _**getPassword**,_ and _**submit**_. 
4. Click at the **Stepper** component and set the following attributes:
   1. **`type`**= _**horizontal**_
   2. **`selected`**= _**getUsername**_ 
   3. **`selectedIndex`** = 0 so that the _**`getUsername`**_ step will come first. 
   4. Now in **`getUsername`** step, drag and drop an Input component to accept username from the user
   5. Drag and drop another **Input** component inside **`getPassword`** step to accept password
   6. Drag and drop a **Button** component inside the **`submit`** step. 
   7. Set the name of the button as _**Login**_. 
   8. Save and run the page.
   9. A **Stepper** component will be displayed with the three steps.

## Associated Attributes

* **`Step Label`**: The name given to a Step. Each Step will have different labels and accepts text values.
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

* **`Label`:** Label of the given step.
* **`Completed`:** A toggle button accepting Boolean values as **`True`** or **`False`** depending on whether step is marked as completed.
* **`Editable`:** A toggle button accepting Boolean value as true or false depending on whether the user can return to this step once it has been marked as completed.
* **`Interacted`:** A toggle button accepting Boolean value as true or false to check whether user has seen the expanded step content or not.
* **`Optional`:** A toggle button accepting Boolean values as true or false, which makes a given step optional.
* **`[stepControl]`:** The top level abstract control of the step.
* **`state`:** State of the step.
* **`Has Error`:** A toggle button accepting Boolean value as true or false to check if ...
* **`errormessage`**: Specify the error message to display if an error occurs.

  \*\*\*\*

**Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

