# Stacked Horizontal Bar Chart

## Overview

A Stacked Horizontal Bar Chart is similar to the normal bar chart with a difference that in a stacked horizontal bar chart, the data values are plotted using a horizontal bar \(row direction\). It provides a good comparison of the data which is placed in the row direction. It is also known as a column chart.

## Usage

A Stacked Horizontal Bar Chart is widely used in industries, health centers, Data analysis, IT companies etc. The use case for stacked horizontal bar chart depends on the scope where it is being used. For example, the insurance companies use this chart to display the report of all the insured clients categorized under male or female in particular years or months, IT \(Information Technology\) companies use this chart for the analysis of the product and service used by their client. Similarly, in the health domain, this chart is used for the treatment analysis and new drugs research data analysis. In all these scopes of the domain, the main use of a stacked horizontal bar chart is for comparison of data categorized on different parameters. There are some other popular use cases where stacked horizontal bar chart is used. Some of them are:

* Insurance companies
* Industries 
* Health centers
* Data analysis

### How to use

1. Open the newly created page.
2. Drag and drop a **Stacked Horizontal Bar Chart** from **Ngx Charts** palette section.
3. Switch to the **Ts** file of the page and then declare the variable and provide values for the dataset. A sample is given below:- 
   * Dataset which consists of all other parameters like labels, and legends. 

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
4. Now switch back to the Html file of the page and provide the dataset array name in the \[datasets\] attribute. For example,

   ```text
        [results] = dataSet
   ```

5. X-axis label can be shown or hidden by providing, `[xAxis] = true` OR `[xAxis] = false`.
6. Y-axis label can be shown or hidden by providing, `[yAxis] = true` OR `[yAxis] = false`.
7. Legends can be shown or hidden by providing, `[legend] = true` OR `[legend] = false`.
8. Save the page and run the application. 

### Example

Consider an industry scenario which records the number of clients who use their products and services. The company plots the data on the stacked horizontal bar chart to get a better comparison. For example,

| Country | Products | Services |
| :---: | :---: | :---: |
| **2016** | 365452 | 265482 |
| **2017** | 345245 | 275825 |

#### Datasets

Here is a sample of a dataset that is declared and initialized in the component class **Ts** file of the project.

```typescript
dataSet = [
  {
    "name": "Products",
    "series": [
      {
        "name": "2016",
        "value": 365452
      },
      {
        "name": "2017",
        "value": 345245
      }
    ]
  },
  {
    "name": "Services",
    "series": [
      {
        "name": "2016",
        "value": 265482
      },
      {
        "name": "2017",
        "value": 275825
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

This legend is taken from the dataset and displayed on the right side of the chart by default. Only the **name** parameter is taken into the legend section.

## Associated Attributes

* **Legends \(Boolean\):** It displays category of data that is used in plotting the stacked horizontal bar chart. If it is true, it shows the legends otherwise it does not show.
* **\[xAxisLabel\] \(String\):** It gives the name to the x-axis.  For example,

  ```typescript
    [xAxisLabel] = "No of Clients"
  ```

* **\[yAxisLabel\] \(String\):** It gives the name to the y-axis.  For example,

  ```typescript
    [yAxisLabel] = "Types of services"
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
* **Value:** It is a value of the key that the user provided manually. For example,
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

* **Results \(object\[\]\):** It provides data to the chart which is plotted on a graph using horizontal bars. For example,

  ```typescript
  dataSet=[
   {
     "name": "India",
     "value": 135148
   },
   {
     "name": "United States",
     "value": 121652
   },
   {
     "name": "Germany",
     "value": 157885
   },
   {
     "name": "France",
     "value": 965782
   },
   {
     "name": "United Kingdom",
     "value": 987564
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

