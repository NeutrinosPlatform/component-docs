# Pie Chart

## Overview

Pie Chart is a circular chart which is divided into different slices each of which represent the corresponding data values.

## Usage

A Pie Chart is widely used in the business world, mass media, product analysis, survey and experimental analysis etc. Consider a health center scenario where a particular hospital wants to plot a chart for the record of its patients admitted to different wards. The chart should indicate the overall hospital and be divided into different sections which represent the wards of the hospital. This can be achieved using a pie chart where a complete pie represents the hospital and divided slices of the pie represent the wards of the hospital. Some of the other popular use cases of line chart are:

* Pharmaceutical Industries \(indicating the different section of drugs\)
* Industries \(for providing information on different products and services \)
* Government offices \(like revenue department\)
* Retails \(for different types of products they provide\)

### How to use

1. Open the newly created page.
2. Drag and drop a **Pie Chart** from the **Ngx Charts** palette section.
3. Switch to the **Ts** file of the page and then declare the variable and provide values for the dataset. A sample is given below: 
   * Dataset which consists of all other parameters like labels, and legends. For example, 

     ```typescript
       ngxpieChartData = [
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
        [results] = ngxpieChartData
   ```

5. X-axis and Y-axis labels can be shown or hidden by providing, `[labels] = true` OR `[labels] = false`.
6. Legends can be shown or hidden by providing, `[legend] = true` OR `[legend] = false`.
7. Save the page and run the application.

### Example

Consider an IT industry which makes a survey on how many users use their products from different parts of the world. The sample data can be recorded as follows:

| Country | Germany | USA | Spain | France | Nepal | India |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Users** | 730000 | 7870000 | 1569558 | 1645553 | 1058048 | 1546488 |

#### Datasets:

Here is a sample of a dataset that is declared and initialized in the component class **Ts** file of the project.

```typescript
ngxpieChartData = [
  {
    "name": "Germany",
    "value": 730000
  },
  {
    "name": "USA",
    "value": 7870000
  },
  {
    "name": "Spain",
    "value": 1569558
  },
  {
    "name": "France",
    "value": 1645553
  },
  {
    "name": "Nepal",
    "value": 1058048
  },
  {
    "name": "India",
    "value": 1546488
  }
]
```

#### Labels:

Here, the labels are automatically taken from the dataset.

#### Legend

Here is a sample of the legend that is declared and initialized in the component class of **Ts** file of the project.

```typescript
 [legend] = true;
```

This legend is taken from the dataset and displayed on the right side of the chart by default. Only the **name** parameter is taken into the legend section.

## Associated Attributes

* **Legends \(Boolean\):** It displays the categories of data that are used in plotting the chart. If it is true, it shows the legends otherwise it does not show.

  ```typescript
    [legend] = true;
  ```

* **xAxisLabel \(String\):** It gives the name to the x-axis.  For example,

  ```typescript
    [xAxisLabel] = "Country"
  ```

* **Labels \(True/false\):** It gives the name to the x-axis and y-axis. These levels are selected from the dataset. If it is true, it shows the x-axis and y-axis levels otherwise it does not show. 
* **explodeSlices \(True/false\):** It gives the radius to each slice. The radius of the slice will be proportional to its value. If it is true, it makes the radius proportional to its values and if it is false, normal slice division is made. 
* **Key:** Key is used to provide user custom key point into the chart. It is like a user’s custom parameter provided to the chart section.
* **Doughnut \(True / False\):** This attribute provides a hollow space at the center of the pie chart. If it is true, the hollow space will be inserted into the chart otherwise not. 
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

* **select \(Events\):** It takes a click event which is done on the slice of the chart. It displays some result on click or on hover of the mouse. For example, displaying data point or the label on click of individual slice.
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
      ngxpieChartData = [
    {
      "name": "Germany",
      "value": 730000
    },
    {
      "name": "USA",
      "value": 7870000
    },
    {
      "name": "Spain",
      "value": 1569558
    },
    {
      "name": "France",
      "value": 1645553
    },
    {
      "name": "Nepal",
      "value": 1058048
    },
    {
      "name": "India",
      "value": 1546488
    }
  ]
  ```

* **fxLayout:** It is a flex layout provided to the chart. It provides different orientation such as row orientation, column orientation to the chart. For example, 

  ```typescript
  fxLayout = 'row' OR fxLayout = 'column'
  ```

* **fxFlex:** It is a directive for fxLayout which is used on it for resizing the elements within the flexbox container flow. It provides three options i.e fxFlex Grow, fxFlex shrink, and fxFlex basis. Here is an example of the implementation of fxFlex.

  ```markup
  <div fxFlex="<grow> <shrink> <basis>"></div>
  ```

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

