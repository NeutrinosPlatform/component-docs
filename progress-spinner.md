# Progress Spinner

## Overview

A Progress spinner component is a circular indicator which is used to indicate progress and activity.

## Usage

A Progress Spinner is a graphical element which is used to show the loading of a process or an activity. The progress spinner keeps spinning until the specified activity is completed.

### How to use

1. Drag and drop a **Progress Spinner** component to the page container. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the required attributes
4. Save and run the page.

### Example

1. Drag and drop a **Progress Spinner** component to the page container. 
2. Double click the component.
3. Input the component field\(s\) with the attribute value\(s\):  

    **`strokewidth`** = _**100**_  

    **`mode`** = _**determinate**_

4. Save it and run.
5. When the page gets loaded, `strokewidth`**100** will be the size of the Progress Spinner component and it will be displayed in **determinate** mode.

## Associated Attributes

* **style:** Accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names. They are defined in the **`Style`**tab as shown below.
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
* **\[mode\]:** Specify the mode of the progress circle. The value should be either `determinate` or `indeterminate`.
* **strokeWidth:** Specify the stroke width of the progress spinner. The value should be a number.
* **\[value\]:** Specify the value of the progress circle. The value should be a number.
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* \[diameter\]: Specify the diameter of the progress spinner.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

