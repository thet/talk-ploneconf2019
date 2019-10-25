<!-- .slide: data-background="green" -->
# $ whoami


<!-- .slide: data-background="green" -->
- Johannes Raggam
- Graz / Austria


<!-- .slide: data-background="green" -->
<img alt="Syslab Logo" title="Syslab.com" style="width: 60%; height: auto" src="./resources/imgs/Logo_SYSLAB_ohneClaim_white_1c.svg" />


<!-- .slide: data-background="green" -->
<img alt="programmatic Logo" title="programmatic.pro" class="antiantialias" style="width: 60%; height: auto" src="./resources/imgs/programmatic-logo-w-200.png" />


<!-- .slide: data-background="green" -->
<img alt="BlueDynamics Logo" title="bluedynamics.com" style="width: 60%; height: auto" src="./resources/imgs/bdan-logo4.svg" />


<!-- .slide: data-background="green" -->
- Plone Foundation Member
- Former Plone Framework Team Member


<!-- .slide: data-background="green" -->
- [https://github.com/thet](https://github.com/thet)
- [https://twitter.com/thetetet](https://twitter.com/thetetet)


<!-- .slide: data-background="green" -->
- [https://thet.github.io/talk-ploneconf2019](https://thet.github.io/talk-ploneconf2019)
- [https://github.com/thet/talk-ploneconf2019](https://github.com/thet/talk-ploneconf2019)




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
Install Vue CLI https://cli.vuejs.org/

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




<!-- .slide: data-background="fuchsia" -->
# About the project "Empower Net"


<!-- .slide: data-background="fuchsia" -->
Organization to help victims in defamation cases.


<!-- .slide: data-background="fuchsia" -->
Offline Space
Online Space


<!-- .slide: data-background="fuchsia" -->
A case is described,
analysed,
strategies are developed,
actions defined
and finally evaluated.


<!-- .slide: data-background="fuchsia" -->
Roles:

- Clients
- Coordinators
- Experts


<!-- .slide: data-background="fuchsia" -->
## More Info

https://empower-net.at/




<!-- .slide: data-background="cyan" -->
# Online Platform


<!-- .slide: data-background="cyan" -->
## Environment Analysis

A few tools available, none fit our use case


<!-- .slide: data-background="cyan" -->
## Why Plone

- Fine grained security
- Powerful workflows
- Hierarchical content
- Instance behaviors (actually not used)
- Own experience


<!-- .slide: data-background="cyan" -->
## Why Vue

- Existing experience
- Experiment with new approach




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


<!-- .slide: data-background="blue" -->
Vue frontend:
https://github.com/thet/bda-empower


<!-- .slide: data-background="blue" -->
Plone backend:
https://github.com/thet/bda.empower




<!-- .slide: data-background="green" -->
# Future


<!-- .slide: data-background="green" -->
vue-plone SDK?


<!-- .slide: data-background="green" -->
Tests?


<!-- .slide: data-background="green" -->
Vue.js 3?




<!-- .slide: data-background="yellow" -->
# React/Volto or Vue?


<!-- .slide: data-background="yellow" -->
Volto: Complete Plone Frontend.


<!-- .slide: data-background="yellow" -->
There is nothing similar in Vue yet.


<!-- .slide: data-background="yellow" -->
Vue for custom applications on top of Plone.


<!-- .slide: data-background="yellow" -->
Matter of taste and experience.




<!-- .slide: data-background="cyan" -->
# That's all folks!

Thank You!




<!-- .slide: data-background="darkviolet" -->
# Ask your questions.
