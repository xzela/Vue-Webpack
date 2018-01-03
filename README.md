# Vue and Webpack

In preparation to using newer technologies, it may be useful to get a high level/basic understanding of how Vue and Webpack work (and work together). I think it's in our best interest that we first attempt to create a simple web app to demonstrate that these tools are:

* Easy to work with
* Easy to understand
* Have some form of support

## Technologies

* [Vue](vuejs.org) (front-end framework)
* [Webpack](https://webpack.js.org/) (bundler tool)
* [Express](https://expressjs.com/) (backend framework)

## History and What's the point?

Vue comes with a [command line tool](https://github.com/vuejs/vue-cli) for creating simple application stubs. I found it to be great for creating simple single page applications and getting the developer up and running. However, once I started  extending beyond the basics, I noticed that the tool hid much of implementation details. This can be problematic if the application stops working (which it did) and I was left searching Google for answers I don't even know the questions to.

I've been playing with Vue and Webpack in preparation for the new Publishing System and quickly realized that both technologies have an incredibly steep learning curve. In fact, from what I can tell, the community is rather small and the avenues for support are limited (mostly StackOverflow and Github issues). Many of the tutorials surrounding Vue are limited to very basic applications and the vast majority depend on the `vue-cli` tool.


## Requirements

Without using the `vue-cli`, create a simple web application that fulfills the following:

### The App
* Create an App that has a `Main` page with a title and heading of `Kinky People`
  * There should be two links: `People` and `Add New Person`
* Create a page called `People` that fetches and lists all of the `Kinky People` from the backend API (ajax request)
  * It would be ideal if it only makes the request once (see Vuex)
* Create a page called `Add New Person` that adds a new name to the `Kinky People` list (ajax request)

### The Technologies
* Use Webpack to bundle the front-end code into a deployable packages
* Use Webpack loaders to allow for transpiling (Vue -> HTML, ES5 -> ES6, Sass/Less -> CSS)
* Use Vue Router to allow for navigation

The data doesn't have to persist (no databases needed).

## Things to consider while


## Bonus

If you have extra time, try completing these tasks:

* Hot module reload. See [vue-loader](https://github.com/vuejs/vue-loader/blob/master/docs/en/features/hot-reload.md)
* Vuex [State Management](https://github.com/vuejs/vuex)
* Figure out how to load images via bundles
