# code-standards
Simple Recommendations for Project Coding Standards

## How to read this file
In each section there will be a short description of why the recommendation has been made and why it may be preferrable to a project. For code styles, you will be presented with two code samples. The first will be the unpreferred code the second will be the preferred. It is up to your team how all of the recommendations should be implemented or not. 

## Origins
There are many ways to come to conclusions about coding styles and best practices. Typically an engineering team should follow the most up-to-date and community backed resources. 

**Best Practice Resources**
- [Airbnb](https://github.com/airbnb/javascript)
- [Google](https://google.github.io/styleguide/jsguide.html)
- [TypeScript Handbook](https://github.com/Microsoft/TypeScript-Handbook/blob/master/pages/Basic%20Types.md)
- [tslint](https://www.npmjs.com/package/tslint)
- [tslint-consistent-codestyle](https://www.npmjs.com/package/tslint-consistent-codestyle)
- [tslint-eslint-rules](https://www.npmjs.com/package/tslint-eslint-rules)
- [tslint-microsoft-contrib](https://www.npmjs.com/package/tslint-microsoft-contrib)


# Pull Requests
It is important to have a common format for describing the code about to enter the base branch so others have context for what they are about to review.

## PR Format
The snippet below is a pretty standard template for pull requests used throughout the development community. Using this template gives a reviewer a good idea of what they are about to review. Context is everything! Don't sell your code short by not giving important details that would prevent remarks to be made by the review. Writing this synopsis of your PR can also ensure that you haven't missed anything from a functional standpoint that allows your code to be tested/reviewed. 
```
### What's this PR do?


### Where should the reviewer start?


### Does this add new dependencies? Is there an installation procedure? (bundle, bower, npm, etc)


### How should this be tested?


### How should this be manually tested?


### Any background context you want to provide?


### Is there a tracking system that can be included?


#### Screenshots
```

## PR Review Guidelines
**Spend at least 1-5 minutes per file**
* Make sure you're being an effective code owner by actively participating in PR Review
* Code review is the first place we can prevent bugs
* Even a one line change can have a code style issue or logic error
* Try to make a comment if you see something that makes you scratch your head OR you see something awesome that the code owner has written.

**Put yourself in the code owner's shoes**
* How would you like your code to be reviewed? It is importatnt to remember that you're reviewing your peer's code.
* Try to be sensitive and understanding that the code written was intentional.
* If you find yourself saying, "I would do this...", take a step back and ask a question instead, "I see that you did this, what is the goal of this code?" or "I like what you did here, did you know this is the ES* way of doing this, which may be more performant... [insert code sample"
* Suggestions with backing from the community are more powerful that opinions. If you're attempting to ask for code changes, especially stylistic, please provide documentation and/or examples popular in the dev community

**Point out logic that may cause errors**
* No one is perfect, there will eventually be errors. Be sure to call out logic issues when seen. 
* As a code owner, please do not hesitate to receive feedback that calls out errors in logic, it's okay to make errors! PR's are check/balances and immediate feedback on code quality to help catch errors that may arise down the road. 

**There is a time and a place for code abstraction**
* Keep in mind that when working in an agile setting, time has been allocated to each ticket. Pending that time allocated to tickets, make suggestions for code improvements that can be completed within the time box. 
* Create a new story for any outstanding work that will be treated as a feature enhancement.
* Add TODO's in your code with a relevant ticket tracking number to ensure that the issues are not forgotten.

**Don't forget to use encouragement for great code**
* If you find some code really awesome while reviewing, make sure you metion it. 
* Emojis are a great way to show someone that you have seen their comments without having to type. I see thumbsup frequently used!

**Suggestions should be formatted questions**
* Try to understand that the developer made a decision for a reason. As a reviewer, when making suggestions, it is important that we don't tell each other to rewrite the core functionality in the code unless it is absolutely necessary (security issue, error prone, etc. Follow suggestions from abstraction section.


# Rebase vs. Merge
This should be a decision made early on in project setting. Choose what is right for the team! 

# Typescript Standards & Usage

# ES6 Standards & Usage

### Trailing commas
Trailing commas make copy and pasting code much easier.
```

```

### Imports


# JsDoc Comments
JSDoc's purpose is to document the API of your JavaScript application or library. It is assumed that you will want to document things like modules, namespaces, classes, methods, method parameters, and so on. More information can be found @: http://usejsdoc.org

There are many standards to format JsDoc comments for classes, functions, interfaces, etc. In the below sections you will see the preferred standard of writing these JsDoc comments.

## Classes

```
/**
 * Represents a book.
 *
 * @constructor
 */
const Book = (title, author) => {
};
```

## Enum 
```
/** 
  * @enum {number} 
  */
enum TRAFFIC_LIGHT = {
  GREEN: 0,
  YELLOW,
  RED,
}
```
or 
```

/** 
  * @enum {number | string} 
  */
enum TRAFFIC_LIGHT = {
  GREEN: "GREEN",
  YELLOW: "YELLOW",
  RED: "RED",
}
```

## Functions

```
/**
 * Converts a number to a string
 * 
 * @method convertNumberToString
 * 
 * @param {Number} [num] - a number that will be converted to a string 
 * @returns {string} - the num as a string
 */
const converNumberToString = (num) => {
  try {
    return String(num);
  } catch (err) {
    throw new Error(`Cannot convert ${num} as a string. Error: ${err}`);
  }
};
```

## Interfaces

```

export interface BookInterface {
  /**
   * A collection of the book's chapters.
   *
   * @type {Array<Chapter>}
   */
  chapters: Array<Chapter>;
  
 /**
   * Total number of pages in the book.
   *
   * @type {number}
   */
  pages: number;
}
```


# File & Variable Naming

# Husky & Git Hooks
