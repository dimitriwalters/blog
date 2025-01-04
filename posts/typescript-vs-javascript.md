---
title: 'When TypeScript is better than JavaScript'
date: '2025-01-04'
---

TypeScript is objectively more safe, less error-prone, and has more features than using plain standard JavaScript. But it doesn't come without cost. It still needs to be compiled to JavaScript to run in the browser. For a large project this may not be a hassle if there's already a build process. But for smaller projects or websites, this can definitely be inconvenient.

What's important to look at when deciding to use TypeScript is what are all the benefits gained, and is that enough to out-weight the setup to use it for smaller projects.

For any project that is mainly making DOM manipulation, using jQuery for example, there's very little benefit gained from using TypeScript instead of JavaScript. You won't be able to take advantage of typings, of classes, generics, because it is not necessary to use OOP for manipulating a webpage. It wouldn't be a bad idea to use TypeScript, but you would basically be writing in plain vanilla JavaScript.

That already covers most simple websites that don't use JavaScript heavily like blogs or a person website.

Here is when TypeScript will be helpful to use:

### Full-Stack Development

I wouldn't say it's 100% beneficial to use TypeScript for full-stack development. Web frameworks have existed before TypeScript took off that were successful in creating complex web applications. But the more complex a codebase gets, the more benefits will be gained from making the code easy to understand. This is where classes, generics, and the typing capabilities of TypeScript will have the most benefits. JavaScript does have classes too, but extra features like generics, static typings, and how much easier it is to write OOP code makes using TypeScript the better choice.

### Writing Libraries

If one library was written in JavaScript, and the exact same library was written in TypeScript, you should probably pick the library written in TypeScript. JavaScript code is extremely vulnerable to bugs and errors. The flexibility of dynamic typings makes coding in JavaScript much more dangerous. Even checking for equality is a dangerous operation in JavaScript. And when writing code for a library or package that will be used by many people in plenty of difference use-cases, this makes it important to have code that is safe and error-prone.

This is where TypeScript's static typings are most useful. Having variables be statically types, having arguments of functions, the return value of a function all statically typed are extra safety precautions that you TypeScript will enforce without having to write extra code yourself. When you combine this capability with custom classes and types, your code becomes much more safe.

### Algorithms

This use-case will sound a bit surprising, because when you think of algorithms you are normally thinking of C++ or Java. Some coders might prefer Python for easy string manipulation and dictionary operations. The main benefit in using a language like Python or JavaScript is how easy it is to use. This is especially important in a coding competition or any task that is timed.

Just like when writing libraries, having error-prone code is a large factor here. Writing algorithms can get really complex really quickly. Something like divide-and-conquer or dynamic programming can become confusing and involve a lot of math. In cases like these, this is when the most amount of errors can be made. The last thing you want when writing an algorithm is to know your code doesn't work because you are using a string instead of an int. This is a time when the cost-benefit of using static typing is worth it, which is when TypeScript is better to use.

These are some of the uses cases of preferring TypeScript over JS and the potential it has to make code easier to write. The next topic will cover how to get the most of TypeScript's large array of features, and some tips that can be use to solve difficult problems.

