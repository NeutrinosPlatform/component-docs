# Area Chart

## Overview

An Area Chart is based on a line chart. The area between the axes and line are colored with different colors, textures, and hatchings.

## Usage

An Area Chart is widely used in comparing data such as the rise and fall of stock market shares. Industries use area charts to display the report of product sales in different geographical regions. IT \(Information Technology\) companies use this chart for the analysis of the products and services used by their clients. Similarly, in the health domain, this chart is used to analyse treatment data. In all these domains, the main use of an area chart is to compare the data categorized by different parameters. There are some other popular use cases where an area chart is used. Some of them are:

* Insurance companies
* Industries 
* Health centers
* Data analysis

### How to use

1. Open the newly created page.
2. Drag and drop an **Area Chart** from **Ngx Charts** palette section.
3. Switch to the **Ts** file of the page and then declare the variable and provide values for the dataset. The sample is given below:- 
   * Dataset which consists of all other parameters like labels, and legends. 

     ```typescript
       dataSet = [
     {
       "name": "Germany",
       "series": [
         {
           "Year": "2010",
           "value": 7300000
         },
         {
           "name": "2011",
           "value": 8940000
         }
       ]
     },
     {
       "name": "USA",
       "series": [
         {
           "name": "2010",
           "value": 7870000
         },
         {
           "name": "2011",
           "value": 8270000
         }
       ]
       }
       ];
     ```
4. Now switch back to the Html file of the page and provide the dataset array name in the \[datasets\] attribute. For example,

   ```text
        [results] = dataSet
   ```

5. X-axis label can be shown or hidden by providing, `[xAxis] = true` OR `[xAxis] = false`.
6. Y-axis label can be shown or hidden by providing, `[yAxis] = true` OR `[yAxis] = false`.
7. Legends can be shown or hidden by providing, `[legend] = true` OR `[legend] = false`.
8. Save the page and run the application.

### Example

Consider an industry which records the data of their product sales from different countries. The company plots the data on the area chart to get a better understanding of variations in sales of products from different countries. For example,

| Country | Germany | USA |
| :---: | :---: | :---: |
| **2010** | 7300000 | 7870000 |
| **2011** | 8940000 | 8270000 |

#### Datasets

Here is a sample of a dataset that is declared and initialized in the component class **Ts** file of the project.

```typescript
dataSet = [
  {
    "name": "Germany",
    "series": [
      {
        "name": "2010",
        "value": 7300000
      },
      {
        "name": "2011",
        "value": 8940000
      }
    ]
  },
  {
    "name": "USA",
    "series": [
      {
        "name": "2010",
        "value": 7870000
      },
      {
        "name": "2011",
        "value": 8270000
      }
    ]
  }
];
```

#### Labels

Here, the labels are automatically taken from the dataset. The label will be **'name'** for the y-axis and **'values'** for the x-axis

#### Legend

Here is a sample of the legend that is declared and initialized in the component class of **Ts** file of the project.

```typescript
 [legend] = true;
```

This legend is taken from the dataset, and displayed on the right side of the chart by default. Only the **name** parameter is taken into the legend section.

## Associated Attributes

* **Gradient \(Color/color hexadecimal code\):** Gradient is a combination of different colors in a pattern. It is used to fill the plotted area in the chart. For example,

  ```css
    background: linear-gradient(to bottom, #33ccff 0%, #ff99cc 100%)
  ```

* **\[xAxis\] \(True/False\):** This attribute diplays the x-axis points. If it is true, the points will be displayed otherwise it won't. For example,

  ```typescript
  [xAxis] = 'True' OR [xAxis] = 'False'
  ```

* **\[yAxis\] \(True/False\):** This attribute diplays the y-axis points. If it is true, the points will be displayed otherwise it won't. For example,

  ```typescript
   [yAxis] = 'True' OR [yAxis] = 'False'
  ```

* **Legends \(Boolean\):** It displays the different categories within the data that is used in plotting the area chart. If the value is true, it shows the legends otherwise it does not show.
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

* **select \(Events\):** It takes a click event which is done on the bars of the chart. It displays some result on click or hover of the mouse. For example, displaying data points and the label when clicking on individual plotted points.
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

* **Results \(object\[\]\):** It provide a data to the chart which is plotted on a graph. For example,

  ```typescript
  dataSet = [
    {
      "name": "Germany",
      "series": [
        {
          "name": "2010",
          "value": 7300000
        },
        {
          "name": "2011",
          "value": 8940000
        }
      ]
    },
    {
      "name": "USA",
      "series": [
        {
          "name": "2010",
          "value": 7870000
        },
        {
          "name": "2011",
          "value": 8270000
        }
      ]
    }
  ];
  ```

* **fxLayout:** It is a flex layout provided to the chart. It provides different orientation such as row orientation and column orientation to the chart. For example, 

  ```typescript
  fxLayout = 'row' OR fxLayout = 'column'
  ```

* **fxFlex:** It is a directive for fxLayout which is used for resizing the elements within the flexbox container flow. It provide three options i.e fxFlex Grow, fxFlex shrink, and fxFlex basis. Here is a example of implementation of fxFlex.

  ```markup
  <div fxFlex="<grow> <shrink> <basis>"></div>
  ```

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

