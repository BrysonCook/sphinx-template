First Draft
===========

With JavaScript being one of the most popular choices for building and designing
websites it is no wonder there are so many different frameworks and libraries
based on it, each with a different take on making JavaScript easier to use or
more powerful. Some of the most popular of these frameworks and libraries include
Angular, jQuery, Next.js, Meteor and the one I will be focusing on React JavaScript.
More specifically the focus of this paper will be to look at a variety of aspects
about React JavaScript and explain why in some situations React is the best library
to use. I will provide an Overview of the unique functionality that the React library
provides to a website and some of the short history of its creation. To end with I
will be providing a short tutorial about how to set up JavaScript and how you can
make your first React webpage. But first lets take a look at how React JavaScript
started and what made it different from some of the other available libraries for JavaScript.



* What is React JavaScript?


React JS was initially created by Jordan Walke, and it is now supported by thousands
of open-source contributors and Facebook. Jordan created React JavaScript in mid 2013
after launching a few early prototypes in 2010 and 2011 [#f1]_. In 2015 React was
considered stable and was starting to be adopted by some major companies including
Netflix and Airbnb, with these large companies supporting React it was not long before
they gained more popularity [#f1]_. By 2016 React was gaining popularity and was a
more widely used JavaScript library by many developers. It had also expanded to
include a wide variety of functionality from the many open-source contributors. Now
React is one of the most popular JavaScript library and is used throughout the world
to create interactive user interfaces.

React allows its users to build modular user interfaces and lets large complex
web based applications change its data without page refreshes [#f2]_. One thing
that makes React different from a lot of the other large frameworks for JavaScript
is that React is not a framework but a library for building composable user interfaces [#f3]_.

Instead of the traditional way that web application were made using templates React
uses components for building the user interfaces. This means that instead of using
basic JavaScript to write out each component of a website every time it is used
React makes it so that you can create each different component once and then call
it wherever it is needed. Another unique aspect of React is when updating data
instead of manually making changes to the DOM, how React manages it is by calling
a render method when it is first initializing and calling render again when the data
is updated. Since this re-render is not a string or a DOM node it is able to complete
the render in about 1ms making it a much faster and easier process then manually
updating DOM nodes [#f3]_.


* How does React work?


A key thing to know about React is that it is not a framework but is instead a
library even though many people compare it to one of the most popular frameworks
Angular. This makes React much easier to work with especially if you are planning
on updating a web app it is not necessary to restart from scratch but instead you
can build out the components over time and have a fully working React web app by
the end of it. Another key distinction to make is that instead of building a React
application you are building a piece of the web page in React and React takes care
of how that one piece of the page functions and renders [#f4]_. Another way
to look at it is that you do not have to have an entire React application but can
instead use React when it is useful within a normal HTML page. A key functionality
of React is its use of components which essentially allow you to re-use sections
of a web app in multiple locations while also allowing them to be slightly different.
I will go more in depth with components later on as they are one of the major pieces
to the React library.

One of the more groundbreaking ways that React works is how it interacts with
the DOM which for now I will just explain it as the Document Object Model and
is a part of JavaScript. What makes what React does different is that instead
of interacting with the DOM directly React creates a new version called the React
virtual DOM. This means when you make changes or write React code you are making
changes the virtual DOM, not the real DOM [#f4]_.

Some sample code to display how components and the React DOM work from [#f5]_
import React from 'react';
import ReactDOM from 'react-dom';

::

    class Car extends React.Component {
      constructor() {
        super();
        this.state = {color: "red"};
      }
      render() {
        return <h2>I am a {this.state.color} Car!</h2>;
      }
    }

    ReactDOM.render(<Car />, document.getElementById('root'));

To give a short explanation of what is going on in the above code, we are essentially
creating a component called Car which has some attribute color which is being set
to red. Below the constructor we have our render which is what is being returned
to the webpage so the user will see “I am a red Car!”. The final aspect of this is
how we are updating the webpage to display this react code and making our changes
to the real DOM since the HTML page is blank apart from a div with the Id of ‘root’.


* How is React different from other frameworks/libraries?


Although the focus of this paper is on React it is still important to know how
it is similar and different from some of the other widely used frameworks and
libraries out there. The two that I will be comparing React to is Angular and
Vue, however the first thing to know is that these three JavaScript tools are not
the same, Angular is a fully fledged from end framework, Vue.js is a progressive
framework, and as we know React is a JavaScript library. Despite this difference
they are still used for almost the same purposes of building front end web applications
using components [#f6]_.

Vue is a framework that focuses on the View layer only but can extend its functionality
with extra packages so that it can also work like an actual framework. Vue lets
you create View components, and combines HTML with special directives and features,
although it is preferred to use Vue’s syntax it is still possible to use raw JavaScript
and JSX in its files. Components in Vue are a bit different in that they are small
and self-contained, meaning that all the HTML, CSS, and JavaScript related to a Vue
component all reside in a file with the .vue extension. The overall use of Vue is
fairly high with an estimated 1 million websites using it. As an overview of the
complexity and learning curve according to Aris Pattakos Vue is the middle of the
road between the three since unlike Angular there is no unique project structure to
learn, but it is still more complex then React [#f6]_.

In the article I found comparing these different tools they decided on comparing
Angular 2 since it is more similar with the use of components. One major difference
between Angular and the others is that Angular is a full framework which means that
it has its own structure which is composed of three things: Modules, Components,
and Services. Another difference is that Angular is built in TypeScript which is
recommended but not necessary as regular JavaScript is also supported. As far as
popularity goes since it was developed by Google it is probably the most well known
out of the three and is also likely the most popular, but this could be biased by
the fact that I searched for this information in Google [#f6]_.

Finally React which being the focus of the paper you would think is the best but
like many tools it has its advantages and disadvantages depending on the type of
web application you are trying to build. But first a comparison between React and
the other two tools mentioned above, as I have mentioned React is a library which
makes it much more flexible then the others and doesn’t enforce any specific project
structure. The main two parts to a React application are the React Elements which
are small building blocks in a React app. Components on the other hand are larger
building blocks that define independent and reusable pieces to be used throughout
the application. As for the language, most people use JSX to create React components
since it is a little more intuitive than JavaScript but anything built using JSX
could also be built with the React JavaScript API. For popularity over 2 million
web sites use React and is one of the more popular JavaScript libraries available [#f6]_.

So how do these three compares, well if you are just starting out and want to use
a powerful tool that allows you to add components to a web page you are better off
using React. In fact, this is the main reason why last semester my group chose to
use React when re-designing a web page instead of trying to learn a more complex
framework like Angular. However like most languages if you spend the time to learn
the syntax any of the three could be used efficiently and affectively to build
reactive web apps using components. Since I have little experience working with
either Vue or Angular it is hard to give a fair comparison between the three but
I still think that the ease of use of React plays a big roll in making it a much
more manageable tool for beginners at least.


* When should you use React?


Even with all the examples of how React is used in an application and some of its
benefits you might still be wondering why should I use React? Well there a multitude
of reasons some of which I have already discussed but will iterate again just to get
the point across that React is a great tool for making amazing web apps. The first
thing I will mention is that React is quite simple and easy to learn compared to
some of the other frameworks and libraries that accomplish similar goals in a web
app. Really the only pre-requisite for React is some understanding of JavaScript
and HTML but even without this knowledge it is still possible to learn and build a
usable React application. The next big advantage to React is its focus on reusability,
what I am referencing here is its use of components which can be used throughout
an application and on multiple pages in the website. This not only saves you time
but like any programming language it simplifies the code by reducing the number of
places that need to be altered when you make a change [#f7]_.

Although it is not a focus of React there are still ways to test and improve its
performance. Some of the ways to inject dependencies automatically include using
ReactJS-di, and if you are just trying to test performance you an use Browserify
or Require JS, however I’m not going to get into much detail on this since I have
almost no idea of how these tools work other than what I was able to read from Nitin
Pandit [#f7]_. As for the testability React is super easy to test since React views can
be treated as functions of the state allowing us to change the state and test the
outputs of different events and functions.

Although I mentioned a few of the reasons to use React earlier there are still many
more situations and reasons why React should be used in the development of web applications.

An example of when to use React is when creating either a header or footer for a
website since this section of the page is likely to stay the same between pages.
An example of a footer from a project I worked on looked something like:

::

    import React from 'react';
    import { useBreakpoint } from '../hooks/useBreakpoint';
    import '../styles/app.css';

    export default function Footer(props) {
      const breakpoints = useBreakpoint();

      if (breakpoints.sm || breakpoints.md) {
        return (
          <div className='footer-mobile' >
            <div className='footer-border'/>

            <div className='footer-text-mobile' key='copyright'>
              &copy; Copyright 2020
            </div>

          </div>
        )
      }

      return (
        <div className='footer' >
          <div className='footer-border'/>

          <div className='footer-text' key='copyright'>
            &copy; Copyright 2020
          </div>

        </div>
      );

    }

What makes this so useful is that now I have the code for a footer in one place
and all I have to do is call this component when I want to add the footer to a new page.


* React specific functionality.


Now that I have shared an overview or React, when to use it, and how to use it I
will get into some of the functionality that comes with React that is different
from what is in regular JavaScript. To begin with I will start with something that
I have already mentioned many times and that is React components. I will spare you
the trouble of reading their uses again but just to summarize they are what makes
React a popular choice of library and have a wide variety of advantages especially
when it comes to reusing code.

The next big functionality that I had mentioned a little earlier is the React DOM
and the differences between the virtual and real DOM. An example of how the React
virtual DOM works with the real DOM in an application. If a user clicks a button
or enters a value in a React component, React compares the state of the virtual
DOM to the real DOM and if they are the same React doesn’t need to do anything [#f4]_.
If they are different that is where React updates the real DOM to match the virtual
one. What this means for the application is that we are able to have complicated
interactions between components that will render without having to reload the page
when a user inputs something or clicks a button [#f4]_. Another advantage is that you don’t
have to worry about the DOM when developing the applications and React will give you
any warnings at compile time.

The next component of React I will discuss is props which is something that I was
confused about for a while and still have a lot to learn about them. But in essence
props allow different components to communicate with each other and pass various
properties between the different components. The part where props become a bit
tricky is that they can only pass information one way, meaning a parent can talk
to its child but not the other way around which can sometimes create some difficulties
when trying to develop complex structures of components communicating between each other [#f4]_.

As a basic explanation of React I will stop there even though there are still a
wide variety of functionalities that are possible in React but are more complicated
and less commonly used.


* How to get Started with React


To finish this paper off I will give a brief tutorial of how to set up and create
your first React application. Most of the information for this will be coming from
the official Reactjs.org page since they have a great tutorial that I used when I
was trying to learn React myself.

One of the best text editors for creating complex web applications in my opinion
is Visual Studio Code since it allows you to go between multiple file types easily
and has many extensions that can be added to make writing code easier and faster.
Two of the extensions I would recommend for anyone who is going to write a lot of
React code would be Prettier and Simple React Snippets, the first one makes your
code much more pleasing to look at and by just saving the file it will re-format
the code so that you have everything aligned and spaced properly. The second one
allows you to generate React templates by simply typing in short codes in a React
file and then it will generate basic templates based on the code you typed in an
example of some of the more useful codes are “imrc” which imports a react component
and “cc” which sets up the component class template for you.

Before starting with React you will need NPM so we will install Node.js which can
be found at nodejs.org/en/
Once we have NPM creating a react application is quite easy all you need to do is
open the terminal, cd into the directory you want your app to be located in and
type the following:

npx create-react-app my-app
cd my-app
npm start

obviously my-app can be replaced with whatever you want your application to be
called but for the purposes of following the tutorial on the React website I just
call it my-app.

After the app has loaded it should open up your web browser with a template of
the React app. I believe it also gives a link to the React page where you can follow
a tutorial. But that about covers how to get your first app up and running.



.. [#f1] Hámori, F. (2020, February 10). The history of React.js on a TIMELINE:
    @RISINGSTACK. Retrieved March 17, 2021, from https://blog.risingstack.com/the-history-of-react-js-on-a-timeline/

.. [#f2] Aggarwal, S. (2018). Modern Web-Development using ReactJS.
    International Journal of Recent Research, 5(1), 133-137.

.. [#f3] Hunt, P. (2013, June 05). Why did we build React? [Web log post].
    Retrieved March 14, 2021, from https://reactjs.org/blog/2013/06/05/why-react.html

.. [#f4] Garner, B. (2020, May 20).
    New to react? You need to understand these key concepts before anything else.
    Retrieved February 12, 2021, from https://levelup.gitconnected.com/new-to-react-you-need-to-understand-these-key-concepts-before-anything-else-2247efc1eaac

.. [#f5] React components. (n.d.).
    Retrieved April 10, 2021, from https://www.w3schools.com/react/react_components.asp

.. [#f6] Pattakos, A. (2021, January 25). Angular vs React vs VUE: Which framework is BETTER? 2021.
    Retrieved April 10, 2021, from https://athemes.com/guides/angular-vs-react-vs-vue/

.. [#f7] Pandit, N. (2019, November 29). What and Why React.js.
    Retrieved February 11, 2021,
    from https://www.c-sharpcorner.com/article/what-and-why-reactjs/#:~:text=React.js%20is%20an%20open,to%20create%20reusable%20UI%20components
