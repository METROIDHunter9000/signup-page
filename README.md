# Signup page

This is a mock sign-up page designed as part of my journey on [The Odin Project](https://www.theodinproject.com/lessons/intermediate-html-and-css-sign-up-form)

This page demonstrates the use of the `<form>` element to collect data from the user. In this example, a flexbox layout & `flex-wrap` are used to lay out the form in a 3x2 grid. (CSS grid likely would have been more appropriate, but at this point in the curriculum it has not been covered)

Some effort was made to ensure this page scales well to smaller displays, but not mobile displays [yet]. This page was tested on a 1920x1080 display and a 1366x768, specifically. The `vw` and `rem` units and the `clamp()` function were used to help achieve better scaling. 

Ultimately these is one detail that yet bothers me: when viewport width is too small, the input elements in the form will undercut their `flex-basis` and `flex-wrap` will fall back one step. In turn this increases the `flex-basis` of the `<main>` element (the right side of the page) which causes vertical overflow out the top of the page. I would like to revisit this problem in the near future and try using CSS grid instead of flexbox for the input form. I expect I will be able to exercise additional rigidity and prevent a vertical overflow.