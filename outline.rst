
In the past I adopted the use of Plone tiles and block layouts in a project instead of crafting full-featured page templates for sites and complex Diazo rules.
Due to the usual project constraints (budget, scope, expertise) we couldn't adopt any of the since then already available JavaScript frontend technologies.
But still, using Plone tiles was a big step forward!
I still wished to be able to use a well defined REST library like plone.restapi for my endpoints for Mockup instead of writing them my own.

For a recent project I didn't want to repeat myself here again. With some Vue.js development experience as background and a strong believe that plone.restapi is hugely important for the future of Plone I switched technologies in a very time and budget constrained project after the first prototype was finished. Because of these unrealistic project parameters, it already didn't matter anyways.

I can't say if it was a good or bad decision. It certainly didn't help the project to finish in time. The project finished in a time which would have been initially acceptable for the projects' scope. But it helped me to better understand the whole framework and come forward. And it gives the user a really nice and snappy user experience.

Now it's ready, see here. Forgive me for unfinished stylings. The functionality is what matters!



vue 3
nuxt
cookbook,
https://vuejs.org/v2/cookbook/dockerize-vuejs-app.html







------------------------------


What about Vue?

Vue got a lot of traction in recent years and it's counted to the top 3 JavaScript frameworks.
It simplicity, flexibility and elegance makes it a first choice among many developers.
In this talk we're going to discuss Vue/Vuex development with Plone and plone.restapi on a real world example.
I'll talk about the Vue ecosystem, Vue design patterns, the pitfalls I trapped in and where Vue can help you.
In the end you might consider using Vue for your Plone frontends instead of Page Templates.





What about Vue?
Using Vue for views.
Replace your views with Vue.


going to show a Vue project which talks with a Plone backend via plone.restapi.
We will discuss some development patterns


In the world of JavaScript where every second a new framework is born Angular, React and Vue are still the biggest players.
While Angular is declining most of the development effort in the Plone community seems to go to the React framework Volto.
This is good.
But there is still Vue and it's probably often the easier to work with.

----

It probably wasn't the best idea to switch from server side rendered browser views to vue in the middle of a side-project run. Or was it? However, the outcome is amazing. A Vue plugin for Plone - or plone.restapi to be specific.

This talk is about the ups and downs using Vue for the whole frontend part of an intranet application, about some tricks when working with Vue and plone.restapi and Vue itself including it's great ecosystem.




==================


About a Project
---------------

I was asked to help develop a portal to support the process of helping victims in harrasment incidents.
The organization focuses more on institutional harrasment, not so much on individual persons. For those other organizations already exist.

So I was aked to help out.
While we were defining the requirements it was somewhat clear to me that Plone was the perfect fit.
(I did not think of using a JavaScript frontend at this point. At least seriously.)
Plone would offer all the security answers we were looking for. All the fine grained control over content permissions. The flexible configurable workflow which was needed. The hierarchical content organization which I love so much (threads, hello).
All that stuff.
All that stuff was already there, except end to end encryption, which would have been nice.
And as we came to define the timeframe of the project, I was asked to deliver it within a month or so.
Well, of course this was impossible.
I told them.
They heard my but I could see in their eyes that they didn't understand. <photo: "grinning people" or "cute cats".
I took the project anyways.

Regarding delivering on time - I failed. I failed for a year.
But now:


Here it is
----------

Video Demo


Vue Plugin Status
-----------------

The Vue plugin doesn't offer the whole Plone editing experience.
As of yet:
No controlpanels,
no content history,
no TTW content types,
no formbuilder.

I doubt it needs to be there.

And you know what?
If you need it go to the <Plone 5.2 screenshot> PMI (Plone Management Interface) or <Volto screenshot> Volto.


Comparisong to Volto
--------------------

Without Volto and especially the plone.restapi, the Vue SDK wouldn't exist.

While Volto focuses to create a full-fledged alternative to Plone based React,
the Vue plugin tries to give you building blocks to create a frontend for a website with editing capabilities, which can be all customized to fit your needs.



The JS framework competition
----------------------------

Vue
React
Angular
Svelte
Mockup
Patternslib


Rough outlines
--------------

some obstacles
: file upload
  Existing libs all implement the server communication, which is a bit weird when using Vuex.
  Dropzone doesn't fully support Promises, apparently (processQueue).

componentization is a form of encapsulating data
  delete file example
    componentization_encapsulation_example.png
    12f5cb9479124c11cfb0a5d6fb55f78c235910e8
    Date:   Wed Sep 18 02:20:08 2019 +0200
    implement delete file


- general tips:

  try to keep your business logic on the backend, in plone.
  
  try to come up with a clever data model and storage strategy.

  try to understand the concepts of Vue and vuex.

  accept apprenticeship fee (lehrgeld)



