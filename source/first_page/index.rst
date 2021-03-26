Introduction to React
=====================

What is React JavaScript?

React JS was initially created by Jordan Walke, and it is now supported by thousands
of open-source contributors and Facebook. Jordan created React JavaScript in mid
2013 after launching a few early prototypes in 2010 and 2011 [#f1]_. In 2015 React was
considered stable and was starting to be adopted by some major companies including
Netflix and Airbnb, with these large companies supporting React it was not long before
they gained more popularity [#f1]_. By 2016 React was gaining popularity and was a
more widely used JavaScript library by many developers. It had also expanded to include
a wide variety of functionality from the many open-source contributors. Now React
is one of the most popular JavaScript library and is used throughout the world to create
interactive user interfaces.
React allows its users to build modular user interfaces and lets large
complex web based applications change its data without page refreshes [#f2]_. One
thing that makes React different from a lot of the other large frameworks for
JavaScript is that React is not a framework but a library for building composable
user interfaces [#f3]_.
Instead of the traditional way that web application were made using templates React uses
components for building the user interfaces. This means that instead of using basic javascript
to write out each component of a website every time it is used React makes it so that
you can create each different component once and then call it wherever it is needed.
Another unique aspect of React is when updating data instead of manually making
changes to the DOM, how React manages it is by calling a render method when it is
first initializing and calling render again when the data is updated. Since this
re-render is not a string or a DOM node it is able to complete the render in about
1ms making it a much faster and easier process then manually updating DOM nodes [#f3]_.


.. [#f1] Hámori, F. (2020, February 10). The history of React.js on a TIMELINE:
    @RISINGSTACK. Retrieved March 17, 2021, from https://blog.risingstack.com/the-history-of-react-js-on-a-timeline/

.. [#f2] Aggarwal, S. (2018). Modern Web-Development using ReactJS.
    International Journal of Recent Research, 5(1), 133-137.

.. [#f3] Hunt, P. (2013, June 05). Why did we build React? [Web log post].
    Retrieved March 14, 2021, from https://reactjs.org/blog/2013/06/05/why-react.html