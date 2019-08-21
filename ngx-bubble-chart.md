# Bubble Chart

## Overview

A Bubble Chart plots the point using a bubble in three dimensions at the same time. The place to plot the data value is determined by the first two dimensions and the corresponding horizontal and vertical axes. The third dimension of the chart represents the size of the individual bubble which depends on the data values.

## Usage

A Bubble Chart is widely used in the business world, mass media, product analysis, survey, experimental analysis etc. Consider a health center scenario where a particular hospital wants to plot a chart to record the number of patients admitted to different wards. The chart should indicate the overall hospital and should be divided into different sections which represent the wards of the hospital. This can be achieved using a bubble chart. Some of the other popular use cases of bubble chart are:

* Pharmaceutical Industries \(indicating the different types of drugs\)
* Industries \(for providing information on different products and services \)
* Government offices \(like revenue department\)
* Retail \(for different types of products provided\)

### How to use

1. Open the newly created page.
2. Drag and drop a **Bubble Chart** from **Ngx Charts** palette section.
3. Switch to the **Ts** file of the page and then declare the variable and provide values for the dataset. A sample is given below:- 
   * Dataset which consists of all other parameters like labels, and legends. For example, 

     ```typescript
       ngxbubbleChartData = [
         {
           "name": "USA",
           "series": [
             {
               "name": "2010",
               "x": 49737,
               "y": 78.8,
               "r": 310
             },
             {
               "name": "2000",
               "x": 45986,
               "y": 76.9,
               "r": 283
             },
             {
               "name": "1990",
               "x": 3706,
               "y": 75.4,
               "r": 253
             }
           ]
         },
         {
           "name": "France",
           "series": [
             {
               "name": "2010",
               "x": 36745,
               "y": 81.4,
               "r": 63
             },
             {
               "name": "2000",
               "x": 34774,
               "y": 79.1,
               "r": 59.4
             },
             {
               "name": "1990",
               "x": 29476,
               "y": 77.2,
               "r": 56.9
             }
           ]
         }
       ]
     ```
4. Now switch back to the Html file of the page and provide the dataset array name in the \[datasets\] attribute. For example,

   ```text
        [results] = ngxbubbleChartData
   ```

5. X-axis label can be shown or hidden by providing, `[xAxis] = true` OR `[xAxis] = false`.
6. Y-axis label can be shown or hidden by providing, `[yAxis] = true` OR `[yAxis] = false`.
7. Legends can be shown or hidden by providing, `[legend] = true` OR `[legend] = false`.
8. Save the page and run the application.

### Example

Consider an insurance company which made a survey of its client located in different parts of the country. The number of clients in a particular area needs to be displayed on a country map using a bubble. For example,

| Data/Area | X | Y | Radius of Circle |
| :---: | :---: | :---: | :---: |
| **Area 1** | 100 | 50 | 20 |
| **Area 2** | 60 | 30 | 10 |
| **Area 3** | 80 | 65 | 15 |

#### Datasets

Here is a sample of a dataset that is declared and initialized in the component class **Ts** file of the project.

```typescript
ngxbubbleChartData = [
  {
    "name": "USA",
    "series": [
      {
        "name": "2010",
        "x": 49737,
        "y": 78.8,
        "r": 310
      },
      {
        "name": "2000",
        "x": 45986,
        "y": 76.9,
        "r": 283
      },
      {
        "name": "1990",
        "x": 3706,
        "y": 75.4,
        "r": 253
      }
    ]
  },
  {
    "name": "France",
    "series": [
      {
        "name": "2010",
        "x": 36745,
        "y": 81.4,
        "r": 63
      },
      {
        "name": "2000",
        "x": 34774,
        "y": 79.1,
        "r": 59.4
      },
      {
        "name": "1990",
        "x": 29476,
        "y": 77.2,
        "r": 56.9
      }
    ]
  }
];
```

#### Labels

Here, the labels are automatically taken from the dataset.

#### Legend

Here is a sample of the legend that is declared and initialized in the component class of **Ts** file of the project.

```typescript
 [legend] = true;
```

This legend is taken from the dataset and displayed on the right side of the chart by default. Only the **name** parameter is taken into the legend section.

## Associated Attributes

* **Legends \(True/False\):** It displays the different categories of the data that is used in plotting the bubble chart. If it is true, it shows the legends otherwise it does not show.
* **Legend Title \(String\):** It gives a title name for the legend which is displayed for the chart. 
* **showGridLines \(True/False\):** It shows or hides the grid lines in the chart. If it is true, it shows lines in the chart otherwise it does not. By default it is true.
* **roundDomains \(True/False\):** It rounds the domain for aligned gridlines in the chart. By default it is false.
* **minRadius \(number\):** It is the minimum bubble radius that is fixed to the chart. It is measured in px. 
* **maxRadius \(number\):** It is the maximum bubble radius that is fixed to the chart. It is measured in px.
* **\[xAxis\] \(True/False\):** This attribute displays the x-axis points. If it is true, it will display otherwise it does not. For example,

  ```typescript
  [xAxis] = 'True' OR [xAxis] = 'False'
  ```

* **\[yAxis\] \(True/False\):** This attribute displays the y-axis points. If it is true, it will display otherwise it does not. For example,

  ```typescript
   [yAxis] = 'True' OR [yAxis] = 'False'
  ```

* **\[xAxisLabel\] \(String\):** It gives the name to the x-axis.  For example,

  ```typescript
    [xAxisLabel] = "Country"
  ```

* **\[yAxisLabel\] \(String\):** It gives the name to the y-axis.  For example,

  ```typescript
    [yAxisLabel] = "No. of Clients"
  ```

* **\[showXAxisLabel\] \(True/False\):** It displays the name that is given to the \[xAxisLabel\]. If it is true, it will display otherwise it does not. For example,

  ```typescript
   [showXAxisLabel]  = 'True' OR [showXAxisLabel]  = 'False'
  ```

* **\[showYAxisLabel\] \(True/False\):** It displays the name that is given to the \[yAxisLabel\]. If it is true, it will display otherwise it does not. For example,

  ```typescript
   [showYAxisLabel] = 'True' OR [showYAxisLabel] = 'False'
  ```

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

* **select \(Events\):** It takes a click event which is performed on the bars of the chart. It displays some result on click or on hover of the mouse. For example, displaying data points and the label when clicking on individual bars.
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

* **Results \(object\[\]\):** It provides data to the chart which is plotted on a graph using bubbles. For example,

  ```typescript
  ngxbubbleChartData = [
    {
      "name": "USA",
      "series": [
        {
          "name": "2010",
          "x": 49737,
          "y": 78.8,
          "r": 310
        },
        {
          "name": "2000",
          "x": 45986,
          "y": 76.9,
          "r": 283
        },
        {
          "name": "1990",
          "x": 3706,
          "y": 75.4,
          "r": 253
        }
      ]
    },
    {
      "name": "France",
      "series": [
        {
          "name": "2010",
          "x": 36745,
          "y": 81.4,
          "r": 63
        },
        {
          "name": "2000",
          "x": 34774,
          "y": 79.1,
          "r": 59.4
        },
        {
          "name": "1990",
          "x": 29476,
          "y": 77.2,
          "r": 56.9
        }
      ]
    }
  ];
  ```

* **fxLayout:** It is a flex layout provided to the chart. It provides different orientation such as row orientation and column orientation to the chart. For example, 

  ```typescript
  fxLayout = 'row' OR fxLayout = 'column'
  ```

* **fxFlex:** It is a directive for fxLayout which is used for resizing the elements within the flexbox container flow. It provides three options i.e fxFlex Grow, fxFlex shrink and fxFlex basis. Here is an example of the implementation of fxFlex.

  ```markup
  <div fxFlex="<grow> <shrink> <basis>"></div>
  ```

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

