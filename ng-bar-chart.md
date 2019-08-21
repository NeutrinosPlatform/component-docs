# Bar Chart

## Overview

A Bar Chart plots the data points using the vertical or horizontal bars providing a good comparison of multiple data points by plotting them side by side. The bar chart includes additional properties over the line chart.

## Usage

A Bar Chart is widely used in the scenario where there is a need for comparison of multiple data points by plotting them side by side. Let’s take a banking scenario where the bank generates a chart on the report of its performance. The report chart should consist of net profit margin, assets, investors, and net bank credit to government \(NBCG\) for different years. The chart should be self-explanatory and should provide good comparison. This can be achieved using the bar chart which plots the data using vertical or horizontal bars. Some of the other popular use cases of bar charts are:

* Industry \(product analysis\)
* Health center \(Disease and cure comparison\)
* Retails \(Sales comparison\)
* Government Surveys \(GDP \(Gross Domestic Product\), PCI \(Per Capita Income\) etc.\)

### How to use

1. Open the newly created page.
2. Drag and drop a **Bar Chart** from **Ng Charts** palette section.
3. Switch to **Ts** file of the page and then declare the variable and provide values for the following in the component class :-
   * A dataset array \(contains y-axis values and labels of the legend\). For example,

     ```typescript
     public barChartData:Array<any> = [
       {data: [65, 59, 55, 81, 56, 55, 40], label: 'Series A'},
       {data: [28, 48, 40, 19, 86, 27, 90], label: 'Series B'}
       ];
     ```

   * A labels array \(contains x-axis values\). For example,

     ```typescript
       public barChartLabels:Array<any> = ['January', 'February', 'March','April', 'May', 'June', 'July'];
     ```

   * Legend value \(either true or false\). For example,

     ```typescript
       public legend = false;
     ```

   * Options value. For example,

     ```typescript
       public barChartOptions:any = {
       responsive: true
       };
     ```
4. Now switch back to Html file of the page and provide the dataset array name in the \[datasets\] attribute. For example,

   ```text
    [datasets] = barChartsData
   ```

5. Provide the labels name in \[labels\] attribute. For example,

   ```text
        [labels] = barChartLabels
   ```

6. Provide the options name in \[options\] attribute. For example, `[options] = barChartOptions`
7. Provide the legend name in \[legend\] attributes. For example, `[legend] = legend`
8. Save the page and run the application.

### Example

Let's take an example of a bank generating a report on different years which includes the performance parameter i.e. net profit margin, assets, investors, and net bank credit to government \(NBCG\).

| Years | Net Profit Margin \(%\) | Assets \(%\) | Investors \(%\) | Net bank credit to govt. \(%\) |
| :---: | :---: | :---: | :---: | :---: |
| **2013** | 69 | 60 | 47 | 23 |
| **2014** | 72 | 64 | 59 | 47 |
| **2015** | 82 | 69 | 65 | 50 |
| **2016** | 79 | 79 | 69 | 55 |
| **2017** | 92 | 60 | 80 | 65 |

#### Datasets

Here is a sample of a dataset that is declared and initialized in the component class **Ts** file of the project.

```typescript
public barChartData:Array<any> = [
   {data: [69, 72, 82, 79, 92], label: 'Net Profit Margin (%)'},
   {data: [60, 64, 69, 79, 60], label: 'Assets (%)'},
   {data: [47, 59, 65, 69, 80], label: 'Investors (%)'},
   {data: [23, 47, 50, 55, 65], label: 'Net Bank Credit to Government(%)'} ];
```

#### Labels

Here is a sample of the labels that are declared and initialized in the component class of **Ts** file of the project.

```typescript
public barChartLabels:Array<any> = ['2013', '2014', '2015','2016','2017'];
```

#### Legend

Here is a sample of the legend that is declared and initialized in the component class of **Ts** file of the project.

```typescript
  public legend=true;
```

#### Options

Here is a sample of the options that are declared and initialized in the component class of **Ts** file of the project.

```typescript
 public barChartOptions:any = {
   responsive: true };
```

## Associated Attributes

* **Label \(String Array\):** Labels are the identity of the data series in a chart. It appears in the legend and tooltips. For example,

  ```javascript
    ChartLabels:Array<any> = ['January', ‘February’, 'March', 'April', 'May', 'June', 'July'];
  ```

* **Datasets \(JSON Objects Array\):** It is a data of the chart which is framed on vertical or horizontal bars. For example,

  ```typescript
  {data: [69, 72, 82, 79, 92], label: 'Net Profit Margin (%)'} ];
  ```

* **chartHover/chartClick \(mouse Events\):** It is an event which appears when the mouse is clicked or placed over the bar chart. For example, displaying label and point value when the mouse is clicked on the chart or mouse is moved over the chart. 
* **Legends \(Boolean\):** It is a name given to the same category of data that is used in plotting the bar chart. If it is true, it shows the legends otherwise it does not show.
* **Color \(Color/color hexadecimal code\):** This property allows user to provide the desired color to the bar chart. For example,

  ```css
    background-color: #92a8d1;
  ```

* **Key:** Key is used to provide user with a custom key point into the chart. It is like a user’s custom parameter provided to the chart section.
* **Value:** It is the value of the key that the user provided manually.
* **Style:** It accepts a string value and affects the different properties \(height, width, color etc.\) of the component based on the values provided \(eg. background: orange; height:200px;\).
* **Class:** "Class" attribute is used to point to a class in a style sheet. A class contains one or more style statements. Classes are created inside the "Style" tab which is opened by selecting the "Style" side menu. The "Class" attribute accepts space-separated class names \(eg. class1 class2\) which are defined in the "Style" tab as shown below.

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

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

