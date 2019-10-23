<!-- .slide: data-background="darkgreen" -->
# $ whoami


<!-- .slide: data-background="green" -->
- Johannes Raggam
- Graz / Austria


<!-- .slide: data-background="lime" -->
- programmatic
- BlueDynamics Alliance Memeber
- Former Plone Framework Team Member
- Since recently: Syslab.com


<!-- .slide: data-background="darkgreen" -->
- [https://github.com/thet](https://github.com/thet)
- [https://twitter.com/thetetet](https://twitter.com/thetetet)
- [http://programmatic.pro](http://programmatic.pro)


<!-- .slide: data-background="darkgreen" -->
- [https://thet.github.io/talk-ploneconf2019](https://thet.github.io/talk-ploneconf2019)
- [https://github.com/thet/talk-ploneconf2019](https://github.com/thet/talk-ploneconf2019)




<!-- .slide: data-background="green" -->
# Project "Empower Net"


<!-- .slide: data-background="green" -->
Organization to help victims in defamation cases.


<!-- .slide: data-background="green" -->
Offline Space
Online Space


<!-- .slide: data-background="green" -->
A case is described,
analysed,
strategies are developed,
actions defined
and finally evaluated.


<!-- .slide: data-background="green" -->
Roles:

- Clients
- Coordinators
- Experts


<!-- .slide: data-background="green" -->
## More Info

https://empower-net.at/




# Online Platform


## Environment Analysis

A few tools available, none fit our use case


## Why Plone

- Fine grained security
- Powerful workflows
- Hierarchical content
- Instance behaviors (actually not used)
- Own experience


## Why Vue

- Existing experience
- Experiment with new approach




<!-- .slide: data-background="yellow" -->
# About Vue

An overview


<!-- .slide: data-background="yellow" -->
## What is it


<!-- .slide: data-background="yellow" -->
it's Vue.js, not Vue.

_But I'll call it Vue._ <!-- .element: class="fragment" -->


<!-- .slide: data-background="yellow" -->
It's pronounced like "View".

_But I say Wue, sorry._ <!-- .element: class="fragment" -->


<!-- .slide: data-background="yellow" -->
## What is it


<!-- .slide: data-background="yellow" -->
Frontend JavaScript library.


<!-- .slide: data-background="yellow" -->
- Reactive
- Component based
- Lifecycle Hooks
- Good Documentation


<!-- .slide: data-background="yellow" -->
- Performant
- Small
- Extensible


<!-- .slide: data-background="yellow" -->
Vue can substitue all your views


<!-- .slide: data-background="yellow" -->
## A simple Example


<!-- .slide: data-background="yellow" -->
### Entry point

TODO: Example code


<!-- .slide: data-background="yellow" -->
### Component

TODO: Example code


<!-- .slide: data-background="yellow" -->
## The Vue ecosystem


<!-- .slide: data-background="yellow" -->
### Vuex


<!-- .slide: data-background="yellow" -->
- Library implementing the state management pattern known by Flux/Redux
- Vue has a one-directional dataflow, like React
- Vuex allows unidirectional data flows by utilizing a central datastore
- Components using vuex get notified by updates


<!-- .slide: data-background="yellow" -->
- Enforces a strict protocol on how to acceess/update data
- Data is stored in ``state``
- Accessed via ``state`` or ``getters``
- Asynchronous operations are ``dispatch``ed
- Data manipulation is ``commit``ed


<!-- .slide: data-background="yellow" -->
TODO: Example code


<!-- .slide: data-background="yellow" -->
### vue-router


<!-- .slide: data-background="yellow" -->
- If your app serves different URL paths, you need a router.
- vue-router defines different entry points to views/components for different URLs


<!-- .slide: data-background="yellow" -->
TODO: Example code


<!-- .slide: data-background="yellow" -->
### vuetify

- Vuetify is a UI library for vue
- There are a lot out there (e.g. Semantic UI for Vue)
- Vuetify is probably the best maintained and popular one


<!-- .slide: data-background="yellow" -->
https://vuetifyjs.com/en/


<!-- .slide: data-background="yellow" -->
TODO: Show Website
https://vuetifyjs.com/en/components/api-explorer


<!-- .slide: data-background="yellow" -->
### nuxt


<!-- .slide: data-background="yellow" -->
NuxtJS is a Vue framework.


<!-- .slide: data-background="yellow" -->
It gives you:

- Server Side Rendering (SSR)
- Static site generation
- Pre-defined configuration
- Best-Practice Project Layout
- Automatic code splitting


<!-- .slide: data-background="yellow" -->
You should consider using it!

_But I don't_ <!-- .element: class="fragment" -->


<!-- .slide: data-background="yellow" -->
## Read this!


<!-- .slide: data-background="yellow" -->
The Vue guide (a must read)

https://vuejs.org/v2/guide


<!-- .slide: data-background="yellow" -->
Vue API documentation

https://vuejs.org/v2/api/


<!-- .slide: data-background="yellow" -->
Vuex Guide

https://vuex.vuejs.org/guide/


<!-- .slide: data-background="yellow" -->
Router Guide

https://vuex.vuejs.org/guide/




<!-- .slide: data-background="blue" -->
# Implementation

A code walk through


## Overview

TODO: folder structure


## Vue Router

- Route to specific views
- Route to ViewFactory


## Vuex Store

- Reactive store, like redux
- Follows specific pattern:
    - State and getters or attribute access
    - Commits for changing attributes
    - Dispatcher for asynchronous changes


## Vue components

- Views = components


## Form elements


## Directives, Filters, Plugins




<!-- .slide: data-background="fuchsia" -->
# What about volto

## What is volto

Volto is a full-featured frontend with the goal to replace the Plone frontend as we know it.


## Comparison to my approach

- vue-plone is a simple, lean framework to get you started.
- It doesn't replace the Plone frontend with all its functionality.
- It's a powerful alternative to server side page template rendering.




<!-- .slide: data-background="cyan" -->
# That's all folks!

Thank You!




<!-- .slide: data-background="darkviolet" -->
# Ask your questions.


