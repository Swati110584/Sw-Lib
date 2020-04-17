*Part 2. Case study - Find a software/lib that uses the testing tool (YTT = Your
Testing Tool)*

*Jest*

Q2.1. What is the purpose of the sw/lib, i.e. what does it aim to do for
users/developers?

Ans - Jest is a JavaScript Testing Framework. [Jest](https://jestjs.io/) is a
JavaScript library for **generating**, **executing**, and **organizing tests**.
Jest is distributed as an NPM package, you can install it in any JavaScript
project. Jest is one of the most popular test runner and also one of the default
choice for Create React App.

Jest is a fast testing framework that's easy to set up. It is developed and used
by Facebook to test all their React applications.

**Jest** helps tests to run automatically. It manages metadata about source code
so it can learn how to run only the relevant test files when a source code file
is changed.

It provides a ‘zero-configuration’ experience and has out-of-the-box features
such as mocking and code coverage. Can apply this testing framework not only
to [React](https://www.thoughtworks.com/radar/languages-and-frameworks/react-js) applications,
but also to other JavaScript frameworks.

1.  **Jest tests can be written faster than traditional ones**:- Advantage of
    Jest tests is that you don’t have to change your test when you update the
    components. It’s because Jest updates the snapshot for you once you agree
    for that.

2.  **Jest tests check if your component behaves correctly**:- Jest gives you a
    powerful tool which allows you to check how your components behave once you
    pass various combinations of props to them. It helps you check if the passed
    data is properly reflected in the component or node tree. Also, you can
    check if the values are correct. You’re able to combine elements from the
    traditional way of testing like mocking functions which are passed as props.
    You can check if component called it as you expected. For example: if you
    want to check whether your component called the fetch function properly. It
    renders information about the fact that it’s fetching the data from the
    API. 

3.  **Jest allows conditional rendering tests**:- Applications are built in a
    way that certain data or functionalities are visible and accessible for
    users according to their permissions, roles etc.

4.  **Visual Diff and Effective Verbosity:-** A big part of good developer
    experience is increasing your productivity. When it comes to testing, when
    tests fail, you want to quickly identify what went wrong with the test. Jest
    has been made very modular and many of its capabilities were moved out to
    individual modules that the community can make use of.

5.  **Relaxed Conventions:-** If you’re coming from different test runners or
    frameworks, you’ll know that they differ in their test suites syntax.

6.  **Test Doubles:-** In automated testing, where we write and execute unit and
    integration tests, it is a common practice to make use of different kinds of
    test doubles to isolate different parts of the system. There are different
    methods of isolation with different goals and behaviors, but they are all
    collectively referred to as test doubles. Jest wraps everything into a
    single entry point called the Mock object (jest.fn). The Mock is accessed
    and used in different ways through the test code, so essentially you don’t
    need to bother yourself with such decisions in your test code about types of
    test doubles. It’s another productivity gain with Jest.

-   It’s easy to learn.

-   It requires zero setup.

-   Managing large test cases is relatively easy because of a snapshot capturing
    feature.

Q2.2. What are the key technologies used to develop the lib?

Ans:- Jest was created by Facebook specifically for testing React applications.
It’s one of the most popular ways of testing React components. Jest is used for
testing both JavaScript front-end and back-end applications.

Many large companies—including Twitter, Instagram, Pinterest, and Airbnb—use
Jest for React testing.

Jest is a delightful JavaScript Testing Framework with a focus on simplicity.

It works with projects
using: [Babel](https://babeljs.io/), [TypeScript](https://www.typescriptlang.org/), [Node](https://nodejs.org/en/), [React](https://reactjs.org/), [Angular](https://angular.io/), [Vue](https://vuejs.org/) and
more!

Jest may be considered a React-specific test runner, in fact it is a universal
testing platform, with the ability to adapt to any JavaScript library or
framework.

-   **Vue.js**: Vue.js is an open-source Model–view–viewmodel JavaScript
    framework for building user interfaces and single-page applications.

-   **AngularJS**: AngularJS is a JavaScript-based open-source front-end web
    framework mainly maintained by Google and by a community of individuals and
    corporations to address many of the challenges encountered in developing
    single-page applications. It can be added to an HTML page with a \<script\>
    tag. AngularJS extends HTML attributes with **Directives**, and binds data
    to HTML with **Expressions**.

-   **Angular**: Angular is a platform for building mobile and desktop web
    applications. Angular is a TypeScript-based open-source web application
    framework led by the Angular Team at Google and by a community of
    individuals and corporations. Angular is a complete rewrite from the same
    team that built AngularJS. 

-   **MobX**: MobX is a battle tested library that makes state management simple
    and scalable by transparently applying functional reactive programming
    (TFRP). The philosophy behind MobX is very simple: Anything that can be
    derived from the application state, should be derived. Automatically, which
    includes the UI, data serialization, server communication, etc.

-   **Redux**: Redux is an open-source JavaScript library for managing
    application state. It is most commonly used with libraries such as React or
    Angular for building user interfaces. A predictable state container for
    JavaScript apps.

-   **Express.js**: Express.js, or simply Express, is a web application
    framework for Node.js, released as free and open-source software under the
    MIT License. It is designed for building web applications and APIs. It has
    been called the de facto standard server framework for Node.js.

-   **GatsbyJS:** Gatsby is a free and open source framework based on React that
    helps developers build blazing fast websites and apps.

-   **Hapi.js:** Build powerful, scalable applications, with minimal
    overhead and full out-of-the-box functionality - your code, your way.

Jest itself is actually not a library but a framework. There’s even a CLI tool
that you can use from the command line. To give an example, the CLI tool allows
you to run only specific tests that match a pattern. Besides that, it hosts much
more functionality, which you can find in the [CLI
documentation](https://jestjs.io/docs/en/cli).

In summary, this means that Jest offers a test runner, assertion library, CLI
tool, and great support for different mocking techniques. All of this makes it a
framework and not just a library.

When you install Jest, you’ll
get [spies](https://codewithhugo.com/jest-fn-spyon-stub-mock/),
in-built [matchers](https://jestjs.io/docs/en/using-matchers), and a huge
mocking library. Since Jest is based on Jasmine, naturally, the tool got all the
great features of Jasmine. Moreover, Jest supports TypeScript, which
makes [Angular testing](https://angular.io/guide/testing) easier. You can also
capture snapshots and perform visual regression testing with the help of Jest.

Every JavaScript project needs an NPM environment (Node has to be installed on
your system). Create a new folder and initialize the project with:

mkdir getting-started-with-jest && cd \$\_

npm init -y

Next up install Jest with:

npm i jest --save-dev

Let's also configure an NPM script for running our tests from the command line.
Open up package.json and configure the script named "test" for running Jest:

"scripts": {

"test": "jest"

},

-   **Easy to Set Up**

Installation of Jest is very simple. All you need to do is:

-   Get [npm](https://www.npmjs.com/get-npm) or [yarn](https://yarnpkg.com/lang/en/) on
    your system.

-   Type this code if you’re using npm:

-   If you’re using yarn, type:

Installation is done!

-   **Speed**

Airbnb is one of the best examples. Earlier they used Mocha for running tests.
When they switched to Jest, on a 32 core system, the runtime of test cases
dropped to 4.5 minutes from 12 minutes. Jest makes your test cases run faster.

-   **Specifications and test-driven development**

Developers like freedom of creativity. But usually there are not many
privileges. Specifications, that is, a written or verbal description of what to
build are to be followed. Super important client needs a **JavaScript function
that should filter an array of objects.**

-   For every object we must check a property called "url" and if the value of
    the property matches a given term then we should include the matching object
    in **the resulting array**. Being a test-savvy JavaScript developer you want
    to follow **test-driven development**, a discipline which imposes to **write
    a failing test before starting to code**.

-   By default Jest expects to find test files in a folder called **tests** in
    your project folder. Create the new folder then:

>   cd getting-started-with-jest

>   mkdir \_*tests*\_

-   Next up create a new file called filterByTerm.spec.js inside tests. You may
    wonder why the extension includes ".spec.". It is a convention borrowed from
    Ruby for marking the file as a specification for a given functionality.

Q2.3. What kind of automated testing tools are used to test the sw/lib
(including but possibly more than YTT) and what are their key features?

Ans:- Test tools can be divided into the following functionalities. Some provide
us with only one functionality, and some provide us with a combination.

1.  **Test launchers** are used to launch your tests in the browser or Node.js
    with user config.

![](https://github.com/Swati110584/Sw-Lib/blob/master/1.PNG?raw=true)

![](https://github.com/Swati110584/Sw-Lib/blob/master/2.PNG?raw=true)

1.  **Testing structure** providers help you arrange your tests in a readable
    and scalable way.

![](https://github.com/Swati110584/Sw-Lib/blob/master/3.PNG?raw=true)



1.  **Assertion functions** are used to check if a test returns what you expect
    it to return and if its’t it throws a clear exception.

![](https://github.com/Swati110584/Sw-Lib/blob/master/4.PNG?raw=true)

1.  **Generate and display test progress and summary**. 

2.  **Mocks, spies, and stubs** to simulate tests scenarios, isolate the tested
    part of the software from other parts, and attach to processes to see they
    work as expected.

3.  **Generate and compare snapshots** to make sure changes to data structures
    from previous test runs are intended by the user’s code changes.

![](https://github.com/Swati110584/Sw-Lib/blob/master/5.PNG?raw=true)

1.  **Generate code coverage** reports of how much of your code is covered by
    tests.

2.  **Browser Controllers** simulate user actions for Functional Tests.

There are several ways to control browsers to simulate user behavior, like
clicking the mouse, drag and dropping, typing, and navigating.

-   Some
    tools install [drivers](https://selenium.dev/documentation/en/webdriver/) that
    are installed on top of them and control the browser using different
    methods. This is how [selenium](https://www.seleniumhq.org/) works:

**Your code on Node.js \<\> WebDriver \<\> FF/Chrome/Safari Driver \<\>
Browser**

-   Another way would be to [inject
    scripts](https://dzone.com/articles/testcafe-e2e-testing-tool) of a JS code
    that has access to the whole application environment: DOM, network, cookies
    etc… to raise events that simulate user behavior. For example, here is how
    you simulate a click:

**document.getElementByID('someButton').dispatchEvent(clickEvent)**

-   Lately, a new way became very popular. Browser maintainers, exposed their
    own native APIs that lets you control the browsers directly. For
    example [puppeteer](https://github.com/puppeteer/puppeteer):

**Your code on Node.js \<\> Browser's API**

1.  **Visual Regression Tools** are used to compare your site to its previous
    versions visually by using image comparison techniques.

*Features*

-   **Performance**- First of all Jest is considered to be faster for big
    projects with many test files by implementing a [clever parallel testing
    mechanism](http://facebook.github.io/jest/blog/2016/03/11/javascript-unit-testing-performance.html).

-   **UI**- Clear and convenient.

-   **Ready-To-Go**- Comes with assertions, spies, and mocks that are equivalent
    to libraries that do the same like [Sinon](https://sinonjs.org/). Libraries
    still can easily be used in case you need some unique features.

-   **Globals**- Like in Jasmine, [it creates test globals by
    default](https://facebook.github.io/jest/docs/en/api.html) so there is no
    need to require them. This can be considered bad since it makes your tests
    less flexible and less controllable, but in most cases it just makes your
    life easier.

![](https://github.com/Swati110584/Sw-Lib/blob/master/6.PNG?raw=true)

-   **Snapshot
    testing**- [jest-snapshot](https://github.com/facebook/jest/tree/master/packages/jest-snapshot) is
    developed and maintained by Facebook, although it can be used in almost any
    other framework as part of the framework’s integration of the tool or by
    using the right plugins.

-   **Great modules mocking**- Jest provides you with an easy way to mock heavy
    modules to improve testing speed. For example a service can be mocked to
    resolve a promise instead of making a network request.

-   **Code coverage**- Includes a powerful and fast built-in code coverage tool
    that is based on [Istanbul](https://github.com/gotwarlost/istanbul).

-   **Reliability**- Since it has a huge community, and used in many very
    complex projects, is considered very reliable.

-   **Support**- It is currently supported by all the major IDEs and tools.

-   **Development**- jest only updates the files updated, so tests are running
    very fast in watch mode.

Q2.4. Which features of the automated testing tools are currently used by the
test suite?

Ans:- For web apps that are based on React, Jest is the preferred framework.
Apart from React, Jest supports unit testing of Angular, VueJS, NodeJS, and
others.

When you install Jest, you’ll
get [spies](https://codewithhugo.com/jest-fn-spyon-stub-mock/),
in-built [matchers](https://jestjs.io/docs/en/using-matchers), and a huge
mocking library. Since Jest is based on Jasmine, naturally, the tool got all the
great features of Jasmine. Moreover, Jest supports TypeScript, which
makes [Angular testing](https://angular.io/guide/testing) easier. You can also
capture snapshots and perform visual regression testing with the help of Jest.

-   **Watch Feature**

### Wouldn’t it be great if a testing tool ran automated test cases whenever you changed the code? Well, your dream comes true with Jest. The frameworks can run in watch mode. All you need to do is run this command in the command-line interface:

After that, Jest will check the app and execute testing whenever you make any
changes in the code.

-   **Test Coverage Reports**

What if you test only 80% of your code? What if by mistake you’re unable to test
the remaining 20%? In that case, chances are that testers may discover some
critical bugs in a later stage. Jest gives you the solution by providing a
built-in coverage report. All you need to do is run this command:

The framework will provide you a test coverage report that shows what percentage
of the code has been tested.

-   **Extensive Mocking**

If you care about fast unit testing, mocking is a vital feature. Mocking helps
you replace dependencies that are slow. Apart from simple mock functions, Jest
helps you to fully control the dependencies in several ways

-   Timer Mocks: Do you want to test a code that fires after a certain time?
    Timer mocks of Jest helps you to test timer related functions, such
    as setInterval() or setTimeOut().

-   ES6 Class Mocks: You can mock all the classes of Ecma 6 script with Jest’s
    help.

-   Manual Module Mocks: Sometimes you may need to replace an entire module
    instead of a few functions. Jest helps you with that. Once you set a manual
    module, the code will target the mock, not the real module.

Jest parallelizes test runs across workers to maximize performance. Console
messages are buffered and printed together with test results. Sandboxed test
files and automatic global state resets for every test so no two tests conflict
with each other.

-   **Immersive watch mode**

Fast interactive watch mode can run only test files related to changed files and
is optimized to give signal quickly. It is very easy to set up and has a few
other options. You can also filter tests by their file names or test names. We
have watch mode working with Mocha, but it isn’t as much powerful. We had to
build our own solution to run specific test folder or file, but this is
something Jest offers for free.

-   **Code coverage**

Jest has a built-in code coverage reports which are a breeze to set up. It is
possible to collect code coverage information from entire projects, including
untested files.

-   **IDE integration**

Jest integrated with PhpStorm using the same config files that are used to be
run from CLI and on continuous integration (CircleCI). It is possible to
navigate with one click to a given test and also to re-run only one test.

-   **Custom reporter integration**

We only need to use a custom reporter to improve integration with Circle CI. It
is possible with Jest
using [jest-junit-reporter](https://github.com/michaelleeallen/jest-junit-reporter).

-   **Snapshots**

The aim of snapshot testing is not to replace existing unit tests, but providing
additional value and making testing painless. In some scenarios, snapshot
testing can potentially remove the need for unit testing for a particular set of
functionalities (e.g. React components), but they can work together as well.

-   **Multi project runner**

Jest team recently introduced a way to run multiple projects together which
would greatly simplify using watch mode and integration with IDEs. 

**Pros:**

-   Simpler API, less boilerplate code.

-   Flexible and easy configuration.

-   Test files executed in isolation.

-   Advanced watch mode.

-   Snapshots support = easier start with testing.

-   Code coverage.

Q2.5. Which features of the automated testing tools are NOT used by the test
suite?

Ans:- Due to its young age, it may also be more difficult to use Jest across the
board for larger projects that utilize different types of testing. For example,
setting up [Nightmare](http://www.nightmarejs.org/) for integration testing. It
is easy to run Nightmare integration tests with Mocha, and the docs have nice
examples. We could have probably gotten Nightmare working with Jest without much
work, but this is an example of the friction you might experience if you want to
integrate Jest across your project stack.

1.  **Browser Controllers** simulate user actions for Functional Tests.

>   There are several ways to control browsers to simulate user behavior, like
>   clicking the mouse, drag and dropping, typing, and navigating.

-   Some
    tools install [drivers](https://selenium.dev/documentation/en/webdriver/) that
    are installed on top of them and control the browser using different
    methods. This is how [selenium](https://www.seleniumhq.org/) works:

**Your code on Node.js \<\> WebDriver \<\> FF/Chrome/Safari Driver \<\>
Browser**

-   Another way would be to [inject
    scripts](https://dzone.com/articles/testcafe-e2e-testing-tool) of a JS code
    that has access to the whole application environment: DOM, network, cookies
    etc… to raise events that simulate user behavior. For example, here is how
    you simulate a click:

**document.getElementByID('someButton').dispatchEvent(clickEvent)**

-   Lately, a new way became very popular. Browser maintainers, exposed their
    own native APIs that lets you control the browsers directly. For
    example [puppeteer](https://github.com/puppeteer/puppeteer):

**Your code on Node.js \<\> Browser's API**

1.  **Visual Regression Tools** are used to compare your site to its previous
    versions visually by using image comparison techniques.

-   **Visual regression testing tools **can also be set up to verify that the
    different screens of your applications are ok visually by a smart comparison
    of screenshots. These

-   screenshots are usually taken as part of your Functional Tests or by
    executing a separate session of browser automation.

![](https://github.com/Swati110584/Sw-Lib/blob/master/7.gif?raw=true)

*Part 3. Interview developers/testers of YTT*  
Q3.1. Reach out to the developers of YTT and ask them about their reasons for
developing YTT. Why this particular type of testing technology? Which situations
is it good for and less good for?

![](https://github.com/Swati110584/Sw-Lib/blob/master/8.png?raw=true)

*Response over chat:-“At Testim, we too are developers and testers, striving to
release quality software faster. We built Testim because writing stable
end-to-end tests was just too hard. We were the first to build an AI-based
functional test automation solution. Since we launched in 2014, we've been
adding features, improving quality, and proving our solution with customers
every day*.”

![](https://github.com/Swati110584/Sw-Lib/blob/master/9.png?raw=true)

Q3.2 Ask them how mature they think YTT is? Is it suitable for use by companies
developing real-world software at scale? Why / why not?

![](https://github.com/Swati110584/Sw-Lib/blob/master/10.png?raw=true)

![](https://github.com/Swati110584/Sw-Lib/blob/master/11.png?raw=true)

Q3.3. Ask them how they plan to evolve and develop YTT going forward. What are
the main improvements needed to take the tool to the next level?

![](https://github.com/Swati110584/Sw-Lib/blob/master/12.png?raw=true)

![](https://github.com/Swati110584/Sw-Lib/blob/master/13.png?raw=true)

![](https://github.com/Swati110584/Sw-Lib/blob/master/14.png?raw=true)
