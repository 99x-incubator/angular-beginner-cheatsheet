# Angular-beginner-cheatsheet
Everything you need to know as a beginner to Angular

Angular has been introduced as a web application development framework which is based on TypeScript and is used for both mobile and web development. This document provides a basic but a proper guidance for the beginners in Angular to grab a overall understanding of what happens with Angular and how to setup and get it up and running.


# Table of Content

 1. Install Angular
 2. Setting up an Angular Project with Angular CLI
 3. Angular LifeCycle Hooks 
 4. Component DOM and attributes
 5. Template Syntax
 6. Communication between components
 7. @ViewChild
 8. Routing
 9. Guarding routes
 10. Modules
 11. Lazy Loading 
 12. Services
 13. Interceptors
 14. Adding UI component libraries
 15. Pipes

## Install Angular

The follwoing methods guides to install Angular to your computer or to downgrade the Angular version at any occurance of such requirement

  **Install Angular (with the latest version)**
  
  Basically you can run the following command

    npm install -g @angular/cli
***or***

If you need to be ascertain about the installation of the latest version, the following is useful

    npm install -g @angular/cli@latest
**NOTE:** **-g** helps to install Angular globally in your computer environment


## Setting up an Angular Project with Angular CLI

 1. **ng new**


Basically, the following command will generate an Angular Project.

    ng new <project-name>

  Running this command will ask you several questions as follows, before setting up the project.
  

    ? Would you like to add Angular routing? (y/N)
    ? Which stylesheet format would you like to use? (Use arrow keys)
    >CSS
    SCSS   [ https://sass-lang.com/documentation/syntax#scss                ]
    Sass   [ https://sass-lang.com/documentation/syntax#the-indented-syntax ]
    Less   [ http://lesscss.org                                             ]
    Stylus [ http://stylus-lang.com                                         ]

  
  

> If  you need to basic routing infrastructure auto-generated, you can simply set **'y'** for the first question.


> You should have to select the stylesheet format you are going to use by simply going *up-and-down with arrow keys* and *press enter* to select

Now your project will be generated after a few minutes


 2. **npm install**
 
* Functionality of `npm install` is to install a package or any packages that it depends on. 
* When an Angular project is generated a **package.json** file will be created. 
* It contains all the dependent packages of the Angular project created 
* Running `npm install` installs the dependencies in the loacl ***node_modules*** folder according to the **package.json** file.
* Make sure to run `npm install` from the ***path*** where package.json is available
 
 
**Depending on the CLI command you insert, you can customize what you do on `ng new`!**

    ng new starter-project --dry-run
--  This will only simulates the process of `ng new <project-name>`, and does not actually generates the files

 
     ng new starter-project --skip-install


    
  -- This skips running the command `npm install` with `ng new`. Thus, you need to run `npm install` after the project generation.

    ng new starter-project --prefix myFirstStep
