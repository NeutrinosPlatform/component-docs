# Guage Chart

## Overview

A Guage Chart uses needles to show the information about the data values on a speedometer. Each section in the gauge needle is colored with a different color and placed on a different axis.

## Usage

A Guage Chart is widely used in executive dashboard reports to show key business indicators. They are useful for comparing small number of variables using multiple needles within the speedometer space.

### How to use

1. Open the newly created page.
2. Drag and drop a **Guage Chart** from the **Ngx Charts** palette section.
3. Switch to the **Ts** file of the page and then declare the variable and provide values for the dataset. A sample is given below: 
   * Dataset which consists of all other parameters like labels and legends. For example, 

     ```typescript
       ngxGaugeChartData = [
     {
       "name": "Germany",
       "value": 40632
     },
     {
       "name": "United States",
       "value": 49737
     },
     {
       "name": "France",
       "value": 36745
     },
     {
       "name": "United Kingdom",
       "value": 36240
     },
     {
       "name": "Spain",
       "value": 33000
     },
     {
       "name": "Italy",
       "value": 35800
     }
        ]
     ```
4. Now switch back to the Html file of the page and provide the dataset array name in the \[datasets\] attribute. For example,

   ```text
        [results] = ngxGaugeChartData
   ```

5. Save the page and run the application.

### Example

Consider an IT company wants a dashboard report to show key business performance indicators of its different branches, so that it can be compared easily with KPI \(Key Performance Indicator\). Here is an example,

| Parameters | KPI |
| :---: | :---: |
| **Germany** | 406323 |
| **United State** | 49737 |
| **France** | 36745 |

#### Datasets

Here is a sample of a dataset that is declared and initialized in the component class **Ts** file of the project.

```typescript
ngxGaugeChartData = [
  {
    "name": "Germany",
    "value": 40632
  },
  {
    "name": "United States",
    "value": 49737
  },
  {
    "name": "France",
    "value": 36745
  }
]
```

#### Labels

Here, the labels are automatically taken from the dataset.

## Associated Attributes

* **angleSpan \(Number\):** It is the angle provided to the gauge spans. The unit is in degrees and the default value is 240 degree.
* **startAngle \(Number\):** It is the angle that the chart is rotated by. It is measured in degrees and the default value is -120 degree. Usually, negative half of the spanning angle \(angleSpan\) is taken to centralize the chart. 
* **units \(String\):** It is the text displayed under the value of the chart data.
* **bigSegments \(Number\):** It is the number of big segments given on the axis collected from the given data set. 
* **smallSegments \(number\):** It is the number of small segments that appear in between every big segment. 
* **min \(number\):** It is the starting point of the scale on the chart from where every data set point starts getting plotted. 
* **max \(number\):** It is the ending point of the scale in the gauge on which the data set values are plotted. 
* **Key:** Key is used to provide user custom key point into the chart. It is like a user’s custom parameter provided to the chart section.
* **Value:** It is a value of the key that the user provided manually.
* **Style:** It accepts a string value and affects the different properties \(height, width, color etc.\) of the component based on the values provided \(eg. background: orange; height:200px;\).
* **Class:** "Class" attribute is used to point to a class in a style sheet. A class contains one or more style statements. Classes are created inside the "Style" tab which is opened by selecting the "Style" side menu. The "Class" attribute accepts space separated class names \(eg. class1 class2\) which are defined in the "Style" tab as shown below.

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

* **select \(Events\):** It takes a click event which is performed on a segment of the chart. It displays some result on click or on hover of the mouse. For example, displaying data points or the label on click of an individual segment.
* **scheme:** It is a color scheme of the chart. For example,

  ```typescript
  let colorSets = [
    {
      name: 'vivid',
      selectable: true,
      group: 'Ordinal',
      domain: ['#647c8a', '#3f51b5', '#2196f3', '#00b862', '#afdf0a', '#a7b61a', '#f3e562', '#ff9800', '#ff5722', '#ff4514'
      ]
    } ];
  ```

* **Results \(object\[\]\):** It provides data to the chart which is plotted on a graph. For example,

  ```typescript
  ngxGaugeChartData = [
    {
      "name": "Germany",
      "value": 40632
    },
    {
      "name": "United States",
      "value": 49737
    },
    {
      "name": "France",
      "value": 36745
    }
  ]
  ```

* **fxLayout:** It is a flex layout provided to the chart. It provides different orientation such as row orientation and column orientation to the chart. For example, 

  ```typescript
  fxLayout = 'row' OR fxLayout = 'column'
  ```

* **fxFlex:** It is a directive for fxLayout which is used for resizing the elements within the flexbox container flow. It provides three options i.e fxFlex Grow, fxFlex shrink, and fxFlex basis. Here is a example of the implementation of fxFlex.

  ```markup
  <div fxFlex="<grow> <shrink> <basis>"></div>
  ```

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

