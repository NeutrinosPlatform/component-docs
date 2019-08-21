# Checkbox

## Overview

Checkbox is rendered by default as square boxes that are checked \(ticked\) when activated. They allow you to select single values for submission in a form.

**Note:** Radio buttons are similar to checkboxes, but with an important distinction — radio buttons are grouped into a set in which only one radio button can be selected at a time, whereas checkboxes allow you to turn single values on and off. When multiple controls exist, radio buttons allow only one of them to be selected, whereas checkboxes allow multiple values to be selected.

## Usage

Checkbox component allows the users to select any combination of options in a group of check boxes. A group of check boxes is used for independent choices. A group of check boxes can also be used to select from a set of one or more choices.

### How to use

1. Drag and drop the **Checkbox** component. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes
4. Save and run the page.

### Example

1. Input the component field\(s\) with the attribute value\(s\):   

    **`class`** = _**check**_  

    **`Id`** = _**check**_

2. Save it and run.
3. When the page is loaded, the `check` class name is pointed to a class in a style sheet and the `id` = **check** is the unique id given for the checkbox. It can be used to apply styles or give reference to point to that particular checkbox.

## Associated Attributes

* **Style:** Accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **Class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names which are defined as shown below:

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

* **Checkbox label:** Display name for the checkbox.
* **value:** Specifies the value attribute of the native input element.
* **required**: Used to check whether the checkbox is required or not.
* **\[\(ngModel\)\]**: Used for two-way data binding. The `ng-model` attribute is used to bind the data in your model into the view which is presented to the user.
* **label**: Is the label given for the checkbox. 
* **id**: A unique id for the checkbox input.
* **name:** Specifies the name for the component.
* **labelPosition:** Specifies whether the label should appear after or before the checkbox. Defaults to 'after'.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* **Checked:** A Boolean value that specifies whether the radio button is checked or not. Choose between `True` or `False`.
* **\(change\)**: Specify the event to be emitted when the group value changes. Change events are only emitted when the value changes due to user interaction with a radio button.
* **Disabled:** A Boolean value that specifies whether the radio button is disabled. Choose between `True` or `False`.
* **Disable Ripple:** A Boolean value that specifies if the ripple is disabled. Choose between `True` or `False`.
* **Indeterminate:** A Boolean value that specifies whether the checkbox is indeterminate. 
  * Choose between `True` or `False`.

{% hint style="info" %}
Note that whenever checkbox is manually clicked, indeterminate is immediately set to **`false`**.
{% endhint %}



\*\*\*\*

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

