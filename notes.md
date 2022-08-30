npx create-next-app next-practice --use-npm 
cd next-practice
Code .

pages folder: 
index.js home page
//cannot import global style sheet directly into components
//global.scss is actually imported into _app.js
//css when imported into page components, the name convention should be xxx.module.css //stylename can be any

routing system: dont have to actually bring in a third party router you dont have to define your routes, just simply put pages inside of pages folder, and all pages are react components.
eg: about page create a file called about.js

rsc + tab    ->      create react components  code snippets

if you create an application with create react app or any regular client-side single page application you are not going to see the content in the source code, you are going to see the main div or the main element where your content is rendered once the javascript loads. so next.js is very for seo

_app.js 
this wraps around all of your page components.
It's just a function takes in a component which is your page props, and just returns that , 
we also could add a layout to this if we want.
we could wrap wrap layout around <Component {...pageProps}>, we can have a header/ afooter/ a navigation whatever you want to show up on every page.
in that layout wen can add to the layer component , and this is the place import any global styles (global.css)

create folder called components:
this is for any components that are not pages. Anytime you want a component where its not going to have its own route/ its own url. you are going to put in here.

create Layout.js in components folder:
convention is to use lowercase for you pages and the uppercase for any other components that you are going to use.
so this layout just going to be a react component. 