# Lab 7

Name: Jeong Min Park


### Q1. Where would you fit your automated tests in your Recipe project development pipeline?

Answer: Within a GitHub action that runs whenever code is pushed

By running tests automatically on every push, bugs can be caught as early as possible. Relying on developers to manually run tests is risky since they might forget to do so. Automating the process ensures consistent test coverage throughout the entire development pipeline.

---

### Q2. Would you use an end to end test to check if a function is returning the correct output?

Answer: No

End-to-end tests are designed to simulate real user workflows, such as clicking buttons and navigating pages. Checking whether a function returns the correct output is the role of a unit test, not an E2E test.

---

### Q3. What is the difference between navigation and snapshot mode?

Navigation mode analyzes a page right after it loads and provides an overall performance metric including JavaScript execution and page load speed. Snapshot mode analyzes the page in its current state and is best used for finding accessibility issues, but cannot measure JS performance or changes to the DOM tree.

---

### Q4. Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.

1. Reduce unused JavaScript: Lighthouse detected an estimated savings of 224 KiB by removing unused JavaScript, which would significantly improve the page load speed.
2. Minify JavaScript: Minifying JavaScript files could save an estimated 23 KiB, reducing the amount of data the browser needs to download and parse.
3. Use efficient cache lifetimes: Setting proper cache lifetimes for static resources could save an estimated 10 KiB and speed up load times for returning visitors.

