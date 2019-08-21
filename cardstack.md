# cardstack

## Overview

This is a swipe-able cards interface which allows user to swipe a stack of cards up, down, left or right. The cards for this example contains static images. When a card is dragged past a point it gets destroyed. This template is responsive across all devices and screen sizes.

## Usage

It can be used in any application that provides a functionality on swipe of cards. It can also be seen in other applications. For example, a shopping cart, where swiping right on a product, adds it to the cart and swiping left, removes the item from the users suggestions list.

### How to Use

1. Download the cardstack template from Neutrinos store.
2. Install the template in N-Studio.
3. When creating a new app select cardstack template from the **ENTER APP DETAILS** menu, and click on the create button.
4. Create a component where you would like to display the cards.

   For example :-  **cardstack component**

5. Import angular2-swing into your component.

   ```text
    import{ StackConfig,
            Direction,
            SwingStackComponent,
            SwingCardComponent } from ‘angular2-swing’;
   ```

6. In **appmodule.ts** import Swing Module

   ```text
   import {SwingModule} from ‘angular2-swing’;
   @Ngmodule({
    imports:[SwingModule]
    })
   ```

7. Define the configurations in your component class and give the allowed directions.

   ```text
    stackConfig:StackConfig = {
      allowedDirections: [Directions.LEFT,
      Directions.RIGHT,
      Directions.UP,
    Directions.DOWN]
    }
   ```

8. If the user swipes a card in a direction that is not specified in the allowedDirections array, the card returns back to its original position once the swipe action is complete.
9. If the user swipes a card in a direction that is specified in the allowedDirections array, the card gets popped out and when it is past a certain threshold it gets destroyed.
10. The allowedDirections array is user Configurable.
11. Import **stackservice** into your component.

    \`import {stackserviceService}

    from../services/stackservice/stackservice.Service\`

12. Inject the stackservice into the **constructor**.

    `constructor(public stackservice:stackserviceService)`

13. When a card is swiped and popped a snackbar appears showing a message containing the direction in which the card was swiped. Depending on the direction in which the card was swiped, the user can perform functionality based on the user's requirement.
14. When a card is popped out the number of cards remaining in the array is shown on the User Interface.
15. Total number of cards remaining in the stack is shown by using a fab in the User Interface and this number can be used to perform functionalities according to the user requirements.
16. Create a new component, drag and drop the custom Html to invoke the cardstack component

    `<bh-cardstack></bh-cardstack>`

    **Support**

17. **Devices:** Android, iOS
18. **Browsers:** Latest version of all modern browsers
19. **Dependencies version:**
    * Angular CLI version: 6.0.0 +
    * Cordova version: 7.1.0 +

