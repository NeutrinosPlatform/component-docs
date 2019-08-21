# Router Outlet

## Overview

Router enables navigation from one view to the next view, as users perform application tasks. Paths can be configured for every page in an app using the Routes editor. These paths specify how a page can be reached.  A Router Outlet acts as a placeholder that Neutrinos Studio dynamically fills based on the current router state. 

## Usage

Router Outlet is used to render a page in a desired location within another page.

### How to use

1. Configure the paths and child paths using the **Routes** editor.
2. Drag and drop the **Router Outlet** component from the **Navigation** section \(of palette components\) inside a page’s container where the routed page should be rendered .

### Example

1. Create two pages namely **home** and **child**.
2. In the **Routes** editor, define a route for the **child** page as a child path of the home component.
3. Create a button component in the **home** page.
4. Set the button’s `routerLink` attribute to the **child** page’s path.
5. Drag and drop the **Router Outlet** component from the **Navigation** section in the **home** page container where the routed page \(child\) should be rendered. Save the changes.
6. Now, when the button is clicked, the **child** page will be rendered where the **Router Outlet** component was placed in the **home** page.

## Associated Attributes

* **Style:** It accepts a string value and affects different properties such as height, width, and color of the component based on the values provided. For example:  `background:orange;height:200px;`.
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
* **\(activate\)**: The event emitter to activate an event.
* **\(deactivate\)**: The event emitter to deactivate an event.
* **isActivated**: A Boolean value used to specify weather the Router Outlet is activated. Choose between `True` or `False`.

## Support

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

