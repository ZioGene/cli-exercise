# cli-exercise

## Angular CLI - SOLUTIONS

Tip: if you don't know what some keyword (for example component) means, you can use `doc` command to learn about it

### Exercise 1
Display Angular CLI version and browser through the help section with a help command.

`ng -v`

### Exercise 2
Create your first project with Angular CLI, explore the folder structure of the new project (Tip: consider to skip installation)

`ng new test-prj -si`

### Exercise 3
Run newly created project to see what was created for you

`ng s -o`

### Exercise 4
Create new component and add it to your entry component (`app.component.html`)

`ng g c new-component`

### Exercise 5
Create new component that is inside the `test` folder, add this component to the `test component`

`ng g c test/component`

### Exercise 6
Create new service that is inside the `test` folder, and provides in app.module (tip: use the flag `--m`)

`ng g s test/my-service --m app.module`

### Exercise 7
Remove semicolon in `app.component.ts` on line 9 and see if this is acceptable by Angular standards using the build in linter

`ng lint`

### Exercise 8
Run both test to be sure that our app is working

`ng test`

`ng e2e`

### Exercise 9
Finally build your application and check out the result

`ng build`

### Exercise 10 BONUS
* Change style type from CSS to SCSS

`ng set defaults.styleExt scss`
* Add custom javascript library and custom css inside your bundled build

add the custom CSS and JS inside the .angular-cli.json relative section:

`"styles": [
      [...add-my-css-library.css...],
      "styles.css"      
    ],
    
    "scripts": [
      [...add-my-js-library.js...],
    ],
    `
