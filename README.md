# JavaScript Testing

## Framework used: Jasmine


**describe** statements are used to identify a suite, which are a group of related specs. It provides a level of indentation.

**it** statements are used to identify a specification ie a container for feature we are testing. If all expectations within a spec return true, it passes. If any of the expectations were to return false, the spec would fail.

**expect** is the launching point of any test. It accepts a single value called the actual function.

**matcher** The comparison method used is called the matcher and is chained after the call to expect. We pass the expected value to the matcher. There are a lot of matcher functions and we can create our own too.

**toBe** tests for strict equality
**not.toBe** can be used to negate a test

**Red Green Refactor cycle**
- You write your tests and they all fail since there's no code to make them pass.
- You then write the code to make your tests pass
- Now you can safely refactor your code and add new features.

**beforeEach(), afterEach()** can be used to remove redundant code

**Testing async code**
We cannot run expect statements inside the callback function as they'll be run within the scope of our application and not the testing framework.

*done()* It signals to the testing framework when an async function has completed.
