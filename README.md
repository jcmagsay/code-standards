# code-standards
Simple Recommendations for Project Coding Standards

## How to read this file
In each section there will be a short description of why the recommendation has been made and why it may be preferrable to a project. For code styles, you will be presented with two code samples. The first will be the unpreferred code the second will be the preferred. It is up to your team how all of the recommendations should be implemented or not. 

## Origins
There are many ways to come to conclusions about coding styles and best practices. Typically an engineering team should follow the most up-to-date and community backed resources. 

**Best Practice Resources**
- Airbnb https://github.com/airbnb/javascript
- Google https://google.github.io/styleguide/jsguide.html 


# Pull Requests
It is important to have a common format for describing the code about to enter the base branch so others have context for what they are about to review.

## PR Format
The snippet below is a pretty standard template for pull requests used throughout the community. 
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
* Spend at least 5 minutes per file
** Code review is the first place we can prevent bugs
** Even a one line change can have a code style issue or logic error
** Make sure you're being an effective code owner by actively participating in PR Review

* Put yourself in the code owner's shoes
** How would you like your code to be reviewed?
** Try to be sensitive

* Point out logic that may cause errors
** No one is perfect, there will eventually be errors. Be sure to call out logic issues when seen. 

* There is a time and a place for code abstraction
** Keep in mind that work has been allocated to 

* Don't forget to use encouragement for great code
** If you find some code really awesome while reviewing, make sure you metion it. 
** Emojis 

* Suggestions should be formatted questions
** Try to understand that the developer made a decision for a reason. As a reviewer, when making suggestions, it is important that we don't tell each other to rewrite the core functionality in the code unless it is absolutely necessary (security issue, error prone, etc)



# Rebase vs. Merge



# ES6

### Trailing commas
Trailing commas make copy and pasting code much easier.
```

```

### Imports


# JsDoc Comments
