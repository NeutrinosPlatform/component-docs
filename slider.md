# Slider

## Overview

The Slider component allows you to select a value from a given range. It has a single handle that can be moved with the mouse or by using the arrow keys. By default, the minimum value of the slider is 0, the maximum value is 100, and the slider moves in increments of 1. These values can be changed by setting the `min`, `max`, and `step` attributes respectively. The initial value is set to the minimum value of the slider.

## Usage

The Slider component is used to select a range of values through mouse, touch, or keyboard. Sliders reflect a range of values along a bar, from which users may select a single value. They are ideal for adjusting volume, brightness, or applying image filters.

### How to use

1. Drag and drop the **Slider** component. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes 
4. Save and run the page.

### Example

1. Drag and drop the **Slider** component. 
2. Double click the component to display the list of attributes.
3. Input the component field\(s\) with the attribute value\(s\): 

    **`invert`** = _**true**_ 

    **`step`** = _**50**_

4. Save and run the page.
5. When the page is loaded the value `invert` = **true** will display an inverted slider and `step`= **50** specifies the step increment value of the slider. In this example, the slider takes two clicks to move to the end of the slider. 

## Associated Attributes

* **Style:** Accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **Class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names which are defined as shown below:
* ```css
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
* **placeholder:** label given to the Slider position.
* **\[\(ngModel\)\]:** Used for two-way data binding. The `ng-model` attribute is used to bind the data in your model into the view which is presented to the user.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* **Invert:** Used to specify whether the slider is inverted. Choose `True` or `False`.
* **Max:** Specify the maximum value that the slider can have. The value should be a number. 
* **Min:** Specify the minimum value that the slider can have. The value should be a number. 
* **Step:** Specify the values at which the slider will slide. The value should be a number. 
* **Show Thumb Label:** Specify whether or not to show the thumb label. Choose `True` or `False`.
* **Vertical:** Specify whether the slider is vertical or not. Choose `True` or `False`.
* **disabled:** Specify whether the component is disabled or not. Choose `True` or `False`.
* **value:** Specify the value of the slider. The value should be either be a number or null. 
* **\(change\):** The event emitted when the slider value is changed.
* **\(input\):** The event emitted when the slider thumb moves.
* **tickInterval**: Specify how often to show ticks. This is relative to the step so that a tick always appears on a step. For example: Tick interval of 4 with a step of 3 will draw a tick every 4 steps \(every 12 values\).

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

