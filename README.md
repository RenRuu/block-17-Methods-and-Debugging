
    node.js = environment to run code outside of the browser
        - cross platform
        - open source server 
        - uses JS

    Facilitates rapid data transfer, allows asynchronous operations, is scalable, and has a large number of free tools.

    Export information from one JS file to another = 'module.exports'

    EX)
        1st file
            //data.js
            
            const supplies = ["firewood", "matches", "tent", "water"];

            module.exports = supplies;

        2nd file
            // index.js

            const supplies = require ("./data.js")

            console.log(supplies);

    
     *Scope* > current context in which variables and expressions can be referenced. 
        - If a variable or expression is not in the current scope, it is not available for use and will return an error.
        - Scopes have a layered hierarchy
            Children have access to parent variables and expressions; However, parents do not have access to their children's.


    Inside > Outside = true / Child to Parent
    Outside > Inside = false / Parent to Child (P's can't access C's information)
        think of "Stay out of my room mom"

    Global 
        - The highest scope, determined by the runtime environment EX) Node.js, a browser.
    Module
        - The scope for code running in a module.
    Functional
        - The scope created within a function.
    Block
        - The scope created with a pair of curly braces.


