# Stripe Follow Along Dropdown

A page built to replicate [Stripe's](https://stripe.com/) dropdown menu. Built for Wes Bos' [JavaScript 30](https://javascript30.com/) course.

[![Screenshot of Stripe Follow Along Dropdown](https://res.cloudinary.com/gerhynes/image/upload/v1517867485/Screenshot_2_aejfea.jpg)](https://gk-hynes.github.io/stripe-follow-along-nav/)

## Notes

In Stripe's menu the dropdowns are seperate elements but there is a div behind them that follows them around and resizes itself.

The lis will be the triggers that will be hovered on. Don't use the anchor link as the trigger or you will move off it every time you try to mouse onto the dropdown.

Select the triggers, the dropdown background div, and the nav.

Make two functions, `handleEnter` and `handleLeave`. Listen for a mouseenter and a mouseleave on each item and trigger these functions.

Whenever you hover over an li, find the content inside it and display it.

Inside `handleEnter`, grab the li and add a class `trigger-enter`. After 150 milliseconds, add a class `trigger-enter-active`.

When you enter into a function, the value of this changes. However, when you enter into an arrow function,the value of this is inherited from the parent function.

By default the dropdown is hidden using `opacity: 0` and `display: none`. You can't go directly from `opacity` 0 to 1 and `display: none` to `display: block`. These can be stepped, however.

When you add a class `trigger-enter` it changes display to block.

After a second, the class `trigger-enter-active` changes opacity to 1.

Inside `handleLeave` remove these classes.
