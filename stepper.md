---
description: A Stepper component is used to divide the content into steps.
---

# Stepper

### Description

Using the Stepper component, a page can be divided into parts. Instead of getting the information at once, it is retrieved in steps. A task can be divided into certain steps and each step will have some actions.

Consider a requirement of creating a login page where username and password should be given before clicking the Submit button. This task can be divided into three steps using the Stepper component. First, get the username, and then the  password, and then finally the Submit option. 

## Usage

1. Drag and drop a **Stepper** component.
2. Fill the required attributes.
3. Save and run the page.

### Example

**Create a stepper with login process:**

1. Drag and drop a **Stepper** component. 
2. Drag and drop three **Step** components inside the **Stepper** component, and input the step label as _**getUsername**_, _**getPassword**_ and _**submit**_ respectively. 
3. Click the **Stepper** component and set **`type`** = _**horizontal.**_
4. In the **getUsername** step, drag and drop an **Input** component to accept username from the user.
5. In the **getPassword** step, drag and drop an **Input** component to accept password.
6. In the **submit** step, drag and drop a **Button** component. Name the button as _**Login**_. 
7. Save and run the page. 
8. A stepper with **getUsername**, **getPassword**, and **submit** label will be displayed.

## Associated Attributes

* **`Stepper Label`**: The name given to a Stepper. Each Stepper

   will have different labels and accepts text values.

* **`style`:** Accepts a string value that affects different properties of the component

   such as height, width, and color, based on the values provided. For example: `background:orange:height:200px`.

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

* **`Linear`:** A Boolean value which can be set to **`True`** or **`False`**. If set to **`True`**, the user will be required  to complete previous steps before proceeding to the next step. 
* **`type`:** Defines the Stepper type. If the stepper is of horizontal type, then set the type as **`horizontal`**. Else, set as the type as **`vertical`**. 
* **`matHorizontalStepper`:** Used to create a horizontal Stepper where the steps will be displayed in horizontal direction. It accepts value **`mat-horizontal-stepper`**.              
* **`matVerticalStepper`:** Used to create a vertical stepper,  where the steps will be displayed in vertical direction. It accepts value **`mat-vertical-stepper`**. 
* **`[selected]`:** Marks the first step to be selected. Give the step label that should be selected by default at the first step. It will contain the label of one of the stepper.
* **`[selectedIndex]`:** Specifies the index of the selected step. This field accepts numbers. The first step is always given  an index value of 0 as the value of index will always be index=position-1. 
* **`(selectionChange)`:** An event emitter that will be emitted when the selected step has changed from previous to next.
* **`(animationDone)`**: Used to specify the event emitted when the current step is done transitioning in.

  \*\*\*\*

**Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 + 

