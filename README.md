# Vue and Webpack


## Background

I've been playing with Vue and Webpack in preparation for the new Publishing System and quickly realized that both technologies have an incredibly steep learning curve. In fact, from what I can tell, the community is rather small and the avenues for support are limited (mostly StackOverflow and Github issues). Many of the tutorials surrounding Vue are limited to very basic applications and the vast majority depend on the `vue-cli` tool.

This Vue [command line tool](https://github.com/vuejs/vue-cli) is used for creating simple application stubs. I found it to be great for creating very basic single page applications and getting the developer up and running. However, once I started  extending beyond the basics, I noticed that the tool hid much of implementation details. This can be problematic if the application stops working (which it did) and I was left searching Google for answers I don't even know the questions to.

In order to facilitate the choice of a good front-end framework, it may be useful to get a high level/basic understanding of how Vue and Webpack work (and work together). I think it's in our best interest to attempt to create a simple web app to evaluate whether these tools are:

* Easy to work with
* Easy to understand
* Have some form of support

## Technologies

* [Vue](vuejs.org) (front-end framework)
* [Webpack](https://webpack.js.org/) (bundler tool)
* [Express](https://expressjs.com/) (backend framework)



## Requirements

Without using the `vue-cli`, create a simple web application that fulfills the following:

### The Express App
* `fetch` route
	* A simple API endpoint that returns an array of names (strings).
* `add` route
	* An API endpoint that simply returns `200` when hit.

### The Vue App
* `Main` page
	* Make the heading for this page `Kinky People`.
	* Add navigation links to the `People` and `Add New Person` pages (see below).
* `People` page
	* Loading this page should fetch and list all of the `Kinky People` from a backend Express API.
	* It would be ideal if it only makes the request once. You are encouraged to use [Vuex](https://github.com/vuejs/vuex) for State Management.
* `Add New Person` page
	* Should feature a form that allows a user to add a new name to the `Kinky People` list (note that this data doesn't actually need to persist - it should simply appear to on the frontend).

### The Technologies
* Use Webpack to bundle the front-end code into a deployable packages
* Use Webpack loaders to allow for transpiling (Vue -> HTML, ES5 -> ES6, Sass/Less -> CSS)
* Use Vue Router to allow for navigation

**Remember:** this is a proof-of-concept; the data doesn't have to persist (no databases needed).

## Things to consider while


## Bonus

If you have extra time, try completing these tasks:

* Hot module reload. See [vue-loader](https://github.com/vuejs/vue-loader/blob/master/docs/en/features/hot-reload.md)
* Figure out how to load images via bundles
