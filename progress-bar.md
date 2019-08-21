# Progress Bar

## Overview

A horizontal Progress Bar is used for indicating progress and activity. It is used to indicate the progress of the work that has been completed.

## Usage

Progress Bar is a graphical control element used to visualize the progression of an extended computer operation, such as file download, file transfer, or installation.

### How to use

1. Drag and drop the **Progress Bar** component to the page container. 
2. Double click the component to display the list of attributes that can be used with it.
3. Fill the attributes which are needed.
4. Save and run the page.

### Example

1. Drag and drop the **Progress Bar** component to the page container. 
2. Double click the component to display the list of attributes.
3. Input the component field\(s\) with the attribute value\(s\):  

    **`value`** = _**55**_  

    **`mode`** = _**determinate**_

4. Save and run the page.
5. When the page is loaded, a Progress bar will be displayed with the value 55 \(indicating the percentage of work completed\) The progress bar is displayed in the `determinate` mode.

## Associated Attributes:

* **style:** Accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. Example: `background:orange;height:200px;`.
* **class:** Used to point to a class in a style sheet. A class contains one or more style statements. Classes are created in the **Styles** editor by clicking  **Styles** in the editor menu. The `class` attribute accepts space separated class names. They are defined in the "Style" tab as shown below:
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
* **\[mode\]:** Specify the mode. Accepted values are:
  * `determinate`\(default\)
  * `indeterminate`
  * `buffer`
  * `query`
* **Color:** A drop-down list which accepts the color based on the angular material theme. You can choose between the following colors, or click the edit button to input the color of your choice:
  * Primary
  * Accent
  * Warn
* **value:** Specify the value of the progress bar. Defaults to zero. Input value should be a number.
* **bufferValue:** Specify buffer value of the progress bar. Defaults to zero. Input value should be a number.
* **\(animationEnd\):** Event emitted when animation of the primary progress bar completes. This event will not be emitted when animations are disabled, nor will it be emitted for modes with continuous animations \(`indeterminate` and `query`\).
* **\[progressbarid\]:** Specify the ID of the progress bar.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

