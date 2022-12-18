# MVC

Project setup: npm install
Compiles & hot-reloads for development: npm run serve
Completes & minifies for production: npm run build

MPA - Multi Page Applications
Classical approach
Page reload on all content changes
Good for large companies with extensive products such as E-Commerce
How it works:
Page is loaded on first site visit
Changes to content must be done through a page refresh
Route changes fetch a separate HTML document for each page
Pros/Cons:
Slower due to page reloads
Interdependent server & client
Strong SEO (Search Engine Optimization) (not dependent on JavaScript)
Stronger information structure
Better Memory Management
More Secure (slightly)

SPA - Single Page Applications
Modern approach
Does not require page reloads
Used by Google, Facebook, Twitter, etc.
How it works:
Page is loaded on first site visit
Content is updated through JSON from the server and rendered through the page
Route changes simply change the content viewed and do not cause a page refresh
Pros/Cons:
Faster load times
Decoupled
Lower SEO (Search Engine Optimization)
More easily mobile friendly
Rendering managed by client creates lighter server load
Caching & Offline Functionality

Component Based Architecture
Small abstracted pieces of the user interface
Can be nested inside of other components to meet complex UI designs
Pages
More complex components comprised of several other nested components
Top level of the component stack that can be used by the Router to render an entire page

What is inside a component:
Template, Script & Style
<template></template>
Used to hold all the HTML for the component
Code can be injected into HTML directly using {{}} aka handlebars
Element attributes can be bound, meaning code can be injected to their values using v-bind or :
Events can be bound into vue using v-on or @

<script></script>

Contains all JavaScript for the component
Must have default export object which contains:
setup() must return an object
Contains the state and any event hooks such as onMounted()
The returned object will contain all the available methods and data for the template
components: {}
Nested components must be imported and added to this object to be used in the HTML

<style></style>

Contains all CSS for component
Can include lang="" attribute to change the styling language
Must include appropriate compilers for this to work
Can include the scoped attribute which will ensure applied css only applies to the components template within the same file

Props & Emit
Props
Data passed down from parent component to child component
Parent passes data as a bound attribute
<child:data="propData">
Captured in child in props property
props:['data']
Can be used directly in template or in setup if passed as first argument
setup(props){props.data}

Reactive & Computed
Reactive:
Reactive objects utilizes the ES2015 Proxy to establish the ability to 'watch' changes
reactive() is for watching full objects as opposed to ref() which is used for watching primitive values
Computed:
Takes in a callback function and returns an immutable reactive ref object
Able to watch reactive objects, when changed function is re-ran and updated value returned

State & AppState
Both State & AppState are reactive objects used to manage data
State is for local component data
Things that are only needed for that component or any of its nested components (ex: 'showForm', 'isActive', 'newData')
AppState is for data shared across multiple components
AppState will be manipulated through services not directly by the component

When using @click the function is called in the return
Class binding :class="{ key(name of class to add): value(boolean condition) ex(vuePoints <= item.price) }"
v-if for if statement v-if="condition", v-else-if="condition" v-else for else condition
v-show="condition", when not true, changes display to none
v-for is a for loop v-for="variable in name of item stored in appstate"

Props are info being passed from a parent to a child
Ex: <team :teamProp="teamData" /> in parent
In child in export default props: ['teamProp'],
Change template values to teamProp
Add props in setup ()
return functions like addPoint(){props.teamProp.score++}
Props get passed as attributes on the component tag

A router link is an <a> tag but instead of using an href it uses to

computed is used to detect whenever there is a change

When submitting a form use @submit.prevent to prevent default
Use emit to notify parent of change

Glossary of Terms
Vue: a frontend javascript framework that makes building user interfaces easier
Component: a .vue file that contains an HTML template, script area for javascript, and a style area for css
Page: a collection and layout of various components
Data Binding: a connection between a property on the component (in the data() return object) and the template
AppState: The AppState utilized the observer pattern and a single source of truth for all components in the app using vue's reactive wrapper
Router: The Vue Router is used to evaluate the address in the url and determine which page should be displayed
V Directives: The special directives for Vue, all being with a v and tell Vue to use some special behind the scene processes. Ex: v-if, v-for, v-show
Reactive: When the data on the page updates automatically based on the state of the application, the user is not required to refresh the page to get the needed data

One Way Data Binding: There is a reactive object called state in our setup method in our components, that works like the appstate but is only used to hold information that is unique to the page. This constructor for this object creates watchers for all its properties allowing the binding process to work. Can bring in properties by referencing them from the state with {{}}

Two Way Data Binding: (data accessed from our html input tag, to our javascript, back to another location in our html)
Ex:
<input v-model="state.myName">

<p>Hello {{ state.myName }},</p>

export default {
name: 'bindings-exercise',
setup() {
const state = reactive({
myName: Name here
})
return {
state
}
}
}

Class Binding with :
Supply values for an attribute within an element. : is used to indicate the following should not be evaluated as a static value, but rather interpreted with a reference to an object
Ex:

<!--The bool adds or removes the class "active" to the element-->
<p :class="{ active: state.isActive }">This text will turn green on active</p>

export default {
name: 'bindings-exercise',
setup() {
const state = reactive ({
//Change the value to true
isActive: false
})
return {
state
}
}
}

<style>
    p {
        color: red;
    }
    .active {
        color: green;
    }
</style>

Lopping over an objects properties:

<div class="blog" v-for="(value, key) in state.blog" :key="key">
    <p>
        {{ key}} : {{ value}}
    </p>
</div>

Computed Properties Ex:
<div class="reverse-message">
    <p>Original Message: {{ state.message }}</p>
    <p>Computed Reversed Message: {{ state.reverseMessage }}</p>
</div>

export default {
    name: 'computed-properties-exercise',
    setup() {
        const state = reactive({
            message: "Hello World!",
            reversedMessage: computed (() => {
                return state.message.split("").reverse().join('');
            }),
        });
        return {
            state
        };
    },
};

Difference between v-if and v-show is that v-if will not render the element to the page in any way. Using v-show means that the element will always be rendered on the page (takes up space) but the condition of the v-show will toggle the display CSS property on the element.

