# Line Chart

## Overview

A Line Chart is a chart which is used to display the data points in connected straight line segments. In the chart, the point is plotted in a way that the point has appeared.

## Usage

A Line Chart is popularly used to chart out trending data. For instance, in stock market share charts. Let us consider a scenario where an Insurance Company wants to track the overall performance of the year along with insured clients and the month. The company chart needs to show the performance of the individual months with the number of clients that are insured. The company KPI \(Key Performance Indicator\) should be able to see the previous data as well as the current data along with the graph indicating the rise or fall of the insured client. In this case, line chart will successfully provide all of these features. Some of the other popular use cases of line chart are:

* Banking
* Health center
* Retail
* Education
* Product Analysis in Industries
* Climate Change Statistic

### How to use

1. Open the newly created page.
2. Drag and drop a **Line Chart** from **Ng Charts** palette section.
3. Switch to the Ts file of the page and then declare the variable and provide values for the following in the component class: 
   * A dataset array \(contains y-axis values and labels of the legend\). For example,

     ```typescript
       public lineChartData:Array<any> = [
       {data: [65, 59, 55, 81, 56, 55, 40], label: 'Series A'},
       {data: [28, 48, 40, 19, 86, 27, 90], label: 'Series B'}
        ];
     ```

   * A labels array \(contains x-axis values\). For example,

     ```typescript
       public lineChartLabels:Array<any> = ['January', 'February', 'March','April', 'May', 'June', 'July'];
     ```

   * Legend value \(either true or false\). For example, 

     ```typescript
       public legend=false;
     ```

   * Options value. For example,

     ```typescript
       public lineChartOptions:any = {
       responsive: true
       };
     ```
4. Now switch back to the Html file of the page and provide the dataset array name in the \[datasets\] attribute. For example,

   ```typescript
    [datasets] = lineChartData
   ```

5. Provide the labels name in \[labels\] attribute. For example,

   ```typescript
    [labels] = lineChartLabels
   ```

6. Provide the options name in \[options\] attribute. For example, `[options] = lineChartOptions`
7. Provide the legend name in \[legend\] attribute. For example, `[legend] = legend`
8. Save the page and run the application.

### Example

Let's take an example of an Insurance company. The KPI \(Key Performance Indicator\) team wants to check the status of the company performance of a particular year, say 2017. Here is the data for the year 2017.

| Months \(2017\) | Jan | Feb | Mar | Apr | May | Jun | Jul | Aug | Sep | Oct | Nov | Dec |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Insured Client** | 13245 | 15401 | 13524 | 9252 | 15025 | 6524 | 8551 | 19321 | 13054 | 15655 | 11024 | 16542 |

#### Datasets

Here is a sample of a dataset that is declared and initialized in the component class **Ts** file of the project.

```typescript
public lineChartData: Array<any> = [
       {data: [8654, 11254, 11958, 13545, 13965, 12548, 13554, 14696, 14979, 16585, 16964, 17015], label: ' Insurance Statistic Year 2017'}];
```

#### Labels

Here is a sample of the labels that are declared and initialized in the component class of **Ts** file of the project.

```typescript
public lineChartLabels:Array<any> = ['Jan', 'Feb', 'Mar','Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec'];
```

#### Legend

Here is a sample of the legend that is declared and initialized in the component class of **Ts** file of the project.

```typescript
  public legend=true;
```

#### Options

Here is a sample of the options that are declared and initialized in the component class of **Ts** file of the project.

```typescript
 public lineChartOptions:any = {
   responsive: true };
```

## Associated Attributes

* **Label \(String Array\):** It is a specific name given to the x-axis and y-axis in the line chart. For example,

  ```typescript
    ChartLabels:Array<any> = ['January', ‘February’, 'March', 'April', 'May', 'June', 'July'];
  ```

* **Datasets \(JSON Objects Array\):** It is a collection of points which is plotted on the line chart using x-axis and y-axis. For example,

  ```typescript
  lineChartData:Array<any> = [
     {data: [65, 59, 55, 81, 56, 55, 40], label: 'Series A'},
     {data: [28, 48, 40, 19, 86, 27, 90], label: 'Series B'},
     {data: [18, 48, 77, 9, 100, 27, 40], label: 'Series C'}declaired
   ]; For example,
  ```

* **chartHover/chartClick \(mouse Events\):** It is an event which appears when the mouse is clicked or placed over the line chart. For example, displaying label and point value when the mouse is clicked on the chart or mouse is moved over the chart. 
* **Legends \(Boolean\):** It is a name given to the same category of data that is used in plotting the line chart. If it is true, it shows the legends otherwise it does not show.
* **Color \(Color/color hexadecimal code\):** This property provides user desired color to the line chart. For example, backgroundColor: ‘rgba\(148,159,177,0.2\)’;
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

  **Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

