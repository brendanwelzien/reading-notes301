# EJS (ExpressJS)

## Getting Started
1. npm init -y in directory file
2. npm install ... express cors ejs, etc.
3. var express = require('express');
4. var cors = require('cors');

5. var app = express(); <-- this creates instance

6. app.use(cors());
7. app.get('/', function(request, response) {
    ....
    response.... <--get route for root directory
});
8. app.set('', path);

9. app.listen(PORT#, function(){

});

## Injecting values into the views
- app.get('/', function(request,response){
    response.render('index');
    *variable: xxxx* <-- insert this in the html
});
## For loops and Arrays
- people: [
    { name: 'brendan'},
    {name: 'brandon'},
]
- in *html* ejs tag,
```js
    ejstag for(var person of people) {
    `<li>`ejstag person.name ejstag `</li>`
    }
```
## If Else Statement
- in *html* ejs tag,
```js
    ejstag for(var person of people) {
        ejstag if(person.name === 'brendan') {ejstag
        }
    `<li>` This is definitely ejstag person.name ejstag `</li>`
    } else { ejstag

   ejstag }
   ```
## Layouts
- layouts are not native, 
- use `npm install --save express-ejs-layouts`
- in server file, add var expressLayouts = require('express-ejs-layouts');
    - app.use(expressLayouts);
- this wraps everything so we can use it in the html
    - ejs-tag body ejs-tag
[<=Back](README.md)

<-- This is my practice pitch for interviews -->
Hi, my name is Brendan Welzien and I was born and raised here in Seattle, Washington. As a recent graduate from the University of Washington, I up until recently was looking for a career in the public health field. This is due to my previous experience working with community stakeholders, including expanding rooftop farms across the Seattle Metropolitan area, assisting food shelters, and working in the restaurant industry. I then shifted my focus into technology as I realized I could leverage not only my life, but others too with software development. This stems from my goal of finding a career that suits my background in public health and in technology. So, I hope to use my knowledge in software development to create applications that promote the general welfare of my communities and those beyond.