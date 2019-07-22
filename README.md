# my-project

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```


DOCUMENTATION OF THE PROJECT
    PACKAGE.JSON
    0. package.json
        It contains scripts on how to run this project and create a build(DIST).
        Also, it has information on dependencies and devDependencies which are used in this project.

    FOLDER Structure
    1. DevOps
        This folder contains files for devops.
    2. DIST
        this folder has production build.
    
    DESIGNING FILE
    3. styles.scss
        WHY SCSS not css
            A. Nested Rules — Nest your CSS properties within multiple sets of {} brackets. This makes your CSS code a bit more clean-looking and more intuitive.

            B. Variables — Standard CSS has variable definitions. So what’s the deal? You can do a lot more with Sass variables: iterate them via a for-loop and generate property values dynamically. You can embed them into CSS property names themselves. It’s useful for property-name-N { … } definitions.

            C. Better Operators. You can add, subtract, multiple and divide CSS values. Sure the original CSS implements this via calc() but In Sass you don’t have to use calc() and implementation is slightly more intuitive.

            D. Functions — Sass lets you create CSS definitions as reusable functions.

            Speaking of which…

            E. Trigonometry(easiest of all) — Among many of its basic features (+, -, *, /) SCSS allows you to write your own functions. You can write your own sine and cosine (trigonometry) functions entirely using just the Sass/SCSS syntax just like you would in other languages such as JavaScript.

            Some trigonometry knowledge will be required. But basically, think of sine and cosine as mathematical values that help us calculate the motion of circular progress bars or create animated wave effects for example.

            F. for-loops, while-loops, if-else statements(easiest of all). You can write CSS using familiar code-flow and control statements similar to another languages. But don’t be fooled, Sass still results in standard CSS in the end. It only controls how property and values were generated. It’s not a real-time language. Only a pre-processor.

            G. Mixins. Create a set of CSS properties once and reuse them or “mix” together with any new definitions. In practice, you can use mixins to create separate themes for the same layout, for example.
    
    CORE STRUCTURE
    4. SRC(FOLDER)
        A. Store(store.js)
            It contains configuration of store and it follows as:
            getters return particular JSON Data w.r.t. to specific functions with the help of
            actions(Api are being called in this) and mutations
        B. router(index.js)
            how the router is working can be configured from here.
        C. Components
            O. Login
                login page with redirect to main screen if successfull
            I. Autocomplete.vue
                It contains a common search bar for searching in inventory w.r.t. navigated page
           II. Dashboard.vue
                It contains navigation panel and logout page with <router-view>
          III. ItemEntry.vue
                It has options to configure vendors and collectors in an inventory management system.
                    In vendor(tab) you can add vendors, items,
                    In Collector(tab) you can assign items to new collectors.
           IV. Tables.vue
                It has options to see vendors and collectors History.
                    In vendor(tab) you can see bills, user name, Total items, Total price, Tax, Grand total, item names, boxes, quanity, price, date of entry etc,
                    In Collector(tab) you can see Receiver board name, board member, date of receiving etc.
           IV. Users.vue
                You can modify the data name w.r.t. Items, Vendors, Receivers, Users and boards.





    Thanking you for reading.


For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
