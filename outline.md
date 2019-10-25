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
Install Vue CLI - https://cli.vuejs.org/

``yarn add @vue/cli``


<!-- .slide: data-background="yellow" -->
Create a project:

``vue create simple-example``


<!-- .slide: data-background="yellow" -->
[src/main.js](./simple-example/src/main.js)

[src/App.vue](./simple-example/src/App.vue)

[src/components/HelloWorld.vue](./simple-example/src/components/HelloWorld.vue)


<!-- .slide: data-background="yellow" -->
## The Vue ecosystem


<!-- .slide: data-background="yellow" -->
### Vuex


<!-- .slide: data-background="yellow" -->
- Central data store
- Flux/Redux state management pattern
- Reactivity, inter-component data exchange


<!-- .slide: data-background="yellow" -->
- Data is stored in ``state``
- Accessed via ``state`` or ``getters``
- Asynchronous operations are ``dispatch``ed
- Data manipulation is ``commit``ed


<!-- .slide: class="full" data-background="yellow" -->
```
import Vuex from "vuex";

export default new Vuex.Store({
  state: {
    name: ''
  },
  getters: {
    name_uppercase(state) {
      return state.name.toUpperCase()
    }
  },
  actions: {
    async GET_NAME({ commit }) {
        let repsponse = await fetch('https://my.webservice/get_name');
        commit('SET_NAME', { value: response.data })'
        return response.data;
    }
  },
  mutations: {
    SET_NAME(state, { value }) {
      state.name = value;
    }
  }
});
```


<!-- .slide: data-background="yellow" -->
### vue-router


<!-- .slide: data-background="yellow" -->
Different URLs to different views


<!-- .slide: class="full" data-background="yellow" -->
```
import Router from 'vue-router';
import Home from '@/views/Home.vue';
import About from '@/views/About.vue';
import Vue from 'vue';

Vue.use(Router);

export default new Router({
  mode: 'history',
  routes: [
    {
      path: "/",
      name: "home",
      component: Home
    },
    {
      path: "/about",
      name: "about",
      component: About
    }
  ]
});

```


<!-- .slide: data-background="yellow" -->
### vuetify


<!-- .slide: data-background="yellow" -->
- UI library
- Material design
- Quite complete


<!-- .slide: data-background="yellow" -->
https://vuetifyjs.com/en/


<!-- .slide: data-background-iframe="https://vuetifyjs.com/en/components/api-explorer" -->


<!-- .slide: data-background="yellow" -->
### nuxt


<!-- .slide: data-background="yellow" -->
NuxtJS is a Vue framework.


<!-- .slide: data-background="yellow" -->

- Server Side Rendering (SSR)
- Static site generation
- Pre-defined configuration
- Best-Practice Project Layout
- Automatic code splitting


<!-- .slide: data-background="yellow" -->
https://nuxtjs.org/


<!-- .slide: data-background="yellow" -->
You should consider using it!

_But I don't_ <!-- .element: class="fragment" -->


<!-- .slide: data-background="yellow" -->
## Read this!


<!-- .slide: data-background="yellow" -->
JavaScript ES6+ changes

E.g: https://www.w3schools.com/js/js_es6.asp


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


<!-- .slide: data-background="blue" -->
## Overview

- Folder structure
- Router
- Store
- Components
- Directives
- Filters
- Plugins




<!-- .slide: data-background="fuchsia" -->
# React/Volto or Vue?


<!-- .slide: data-background="fuchsia" -->
Volto: Complete Plone Frontend.


<!-- .slide: data-background="fuchsia" -->
There is nothing similar in Vue yet.


<!-- .slide: data-background="fuchsia" -->
Vue for custom applications on top of Plone.


<!-- .slide: data-background="fuchsia" -->
Matter of taste and experience.




<!-- .slide: data-background="cyan" -->
# That's all folks!

Thank You!




<!-- .slide: data-background="darkviolet" -->
# Ask your questions.


