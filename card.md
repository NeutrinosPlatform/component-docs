---
description: >-
  Card is a versatile container which can be used to display a  wide variety of
  content including static images, dynamic images, panels, text, and actions,
  all pertaining to a single topic.
---

# Card

## Description

Card can contain many sub-components such as card title, card subtitle, card image, card action, card header, and card footer. These sub-components can be inserted within a card by clicking on the add options provided at the bottom of the card. Further, each sub-components component can be sorted within a card according to your application requirements. Also, properties of each sub-component can be configured by clicking on the component and updating its Attribute window.

Therefore, you can call Card as a lead component which groups all card sub-components together and displays it as a single block. 

When you add a Card component to a page container, by default, sub-components such as the card title, card sub-title, card image, card content, and card action are already added within the Card.

You can also add other palette components into a Card. For example, you can add a Row component to a card and configure its behavior.

### Usage

1. Drag and drop a **Card** component to a page container.
2. \(optional\) Add sub-components such as **card-header, card-title, card-subtitle, card-image, and card-actions** to the **Card** by clicking respective options at the bottom of the card.
3. Click the respective component and set its attributes/behavior using the Attributes window.

### Example

**Display a Card with a title, image, and a paragraph:**

1. Drag and drop a **Card** component to the page container. 
2. Select the **Card Title** component inside the card. In the card title Attributes window, set the **`card title`** as _**Blog**_. 
3. Now, click the **Card Image** component. In the Attributes window, enter _**assets:\android\wallpaper.jpg**_ in the **`Assests src`** field. This sets the path of the image to the image stored in assets folder. 
4. Save and run the page.
5. A **Card** component ****with the title as _**Blog**_, and a wallpaper image will be displayed on the screen.

## Associated Attributes:

#### **Basic Properties: These properties remain the same for all Card components.**

* **`style`:** Accepts a string value that affects different properties of the Card such as height, width, and color, based on the values provided. For example: `background:orange:height:200px`.
* **`class`:** Used to point to a class in a style sheet.  Each class contains one or more style statements defined in the **Style** editor. The `Class` field accepts space separated class names such as `class1 class2` , where each class is defined in the Style editor as shown below:

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

### Other Properties: These properties are unique to each component.

### Card:

* **`card label`:** Display name of the Card.
* **`tabindex`:** Specifies the index of the selected Card sub-component.

### Card Title:

A Card Title can be used to give a title to any block. It contains a text value.

* **`Title`:** Title of the Card. This field accepts string value and displays the inserted value as the card title, applying bold property. 
* **`Align`**: Select an alignment from the drop-down list to align the Card Title.
  * **`Right`**: Aligns the card title to right.
  * **`Left`**: Aligns the card title to left.
  * **`Center`**: Aligns the card title to the center of the Card.
  * **`Justify`**: defines how the browser distributes space between and around content items along the main-axis of a flex container, and the inline axis of a grid container.

### Card Sub-Title:

A Card Sub-Title can be used to give a subtitle to any block. It contains the text value. It is used below the title component.

* **`Sub Title`:** Sub-title of a card. This field accepts string value and displays it as the card sub-title on the page. 
* **`Align`**: Select an alignment from the drop-down list to align the card title to right, left, center, or justify. 

### Card Image:

A card image component can be used to display an image inside the card.

* **`alt`**: Alternate text for the image. This text will be displayed instead of the image when the image does not load.  For example, alt text can be _Image not available_.
* **`Assets src`**: Stores the source path of the image. It displays the image if the image is present in the path that is specified. For example: _**android\wallpaper.jpg**_ ****displays the image which is in **.jpg** format. 
* **`[src]`**: The source location of the image.
* **`Secure URL`**: The Secure URL of the image.  If you do not use a secure URL, app users may get warnings that the app contains insecure data.
* **`[collection name]`**: 
* **`[image filter]`**:

### Card Content:

A card content is a container in which you can insert a paragraph or text. It is basically intended to display a block of text. 

You can add other palette components into a card content.

* **`Align`**: Select an alignment from the drop-down list to align the card title to right, left, center, or justify. 
  * Justify defines how the browser distributes space between and around content items along the main-axis of a flex container, and the inline axis of a grid container.

### Card Action:

A card action can be used as a container of buttons, where in clicking a button should perform some action.

* **`Align`**: Select an alignment from the drop-down list to align the card title to right, left, center, or justify. 
  * Justify defines how the browser distributes space between and around content items along the main-axis of a flex container, and the inline axis of a grid container.

### Card Header:

A card header contains the card title, card subtitle, and card image as attributes within it. It cannot contain any other component inside it.

Multiple card headers can be inserted to a card.

* **`title`**: Accepts string value and the text will be displayed as the title of the card in bold property.
* **`subtitle`**: Accepts string value and the text will be displayed below the title attribute in normal text. 
* **`Assets src`**: This attribute stores the path of the image stored in the system and it displays the images based on the path \(if present\). 
* `[src]`:
* **`alt`**: Alternate text for the image. This text will be displayed instead of the image when the image does not load.  For example, alt text can be _Image not available_.
* **`[src]`**: The source location of the image.
* **`Secure URL`**: The Secure URL of the image.  If you do not use a secure URL, app users may get warnings that the app contains insecure data.
* **`[collection name]`**: 
* **`[image filter]`**:

### Card Footer:

A card footer component can be used where the data should be displayed as footer, at the bottom of any container. It can contain data such as string value, logo or any content inside it.

* **`card label`:** Name of the card.
* **`tabindex`:** Specifies the index of the selected Footer component.

**Support**

* **Devices:** Android, iOS
* **Browsers:**  Latest version of all modern browsers
* **Dependencies version:** 
  * Angular CLI version: 6.0.0 + 
  * Cordova version: 7.1.0 +

