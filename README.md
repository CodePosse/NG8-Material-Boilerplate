
  

  

# NG8-Material-Boilerplate :dash:

  

  

## Welcome to the boilerplate

  

  

My goal was to make something to kick-start someone on making an Angular 2-8 (this app is 8.3.0) with the latest Material Design without much prior knowledge.

  

  

> Do Google things on Google Stuff

  

  

Recently as a TVC (contractor) for Google, I was asked to mentor some [UXRs](go/uxr) (UX researchers) that were not technical, but needed to get started with cut and paste while understanding context, so I enhanced this for a version I have internally. This also works for people that are just stuck and frustrated and think that the lack of readable documentation in the public areas is borderline criminal. :cop: A lot of documentation is written like it is in advanced Latin while we are learning French in Jr High. Bad Karma.

  

  

Google has plenty of internal tools and learning facilities, this is more of a passion project that does not require their tools like [Acey](go/acey), [ACX](go/acx), or [Dart](https://dart.dev/). While having access to all that is awesome, as a TVC I was not able to use any of it and had to make everything from scratch. :man_facepalming:

  

  

## Getting started
- It's a good idea to make a copy of `demo-app` and name it whatever you want
- Ok, so you have a new folder. Open a terminal window or if you are on Windows you have PowerShell. You hold `shift + right click` and in the menu you will see "Open with PowerShell".
- You are now at the command line
- You need to install Angular CLI (command line interface) so you will type `npm install -g @angular/cli`
- We will need to install all the dependencies by typing in `npm install` and it will take a few moments for it to get everything it needs.
- If you type `ng serve --open` you will start up Angular and automatically open up a browser window to the project.
  

### Overview

  

The vast majority of the modules you will need are included and placed in a TypeScript file called `material.ts` inside the `demo-app/` folder. When you get started, it is a good idea to make your own copy of this folder and start your work there.

  

  

Like mentioned above, the `demo-app/` folder contains most of the Angular Material components imported, but NOT used in any context yet. You can go to the [Angular Material](https://material.angular.io/components/categories) homepage and get copy-and-paste examples of the components. To see what items are available, you can open the `material.ts` file and see the names of the modules that are imported.

  
### What you get
This is pretty minimal, but it should help. 
- I have the majority of Angular Material components readily available for you to use. Just copy-paste them from [Angular Material](https://material.angular.io/components/categories).
- I use the default indigo-pink Material theme in `styles.scss` but you can change it later.
- I have included Material Icons by linking from `index.html`
- I have created a header and footer and used Material Design's `<mat-card>` wrapping a piece of text to let you know they are working.

#### Angular basic commands

  



  

  

##### Run your app

  

Start the app: `ng serve` and open your browser to: http://localhost:4200

  

-or-

  

Start the app and open a browser automatically: `ng server --open`

  

  

Once it is running it will stay running until you force it to quit. Mac will be `command+c` Windows will be `ctrl+c`. While running, everytime you save a file, Angular will rebuild and refresh the browser without you needing to hit refresh.

  

  

#### Adding components

  

While the server is not running, you can create some components. For this first part, we will create a test component to be used across the whole site in the same place. I have already created a header and footer you can find inside the `src/` folder as a reference, but let's make a new one from scratch!

  

To create a test item, we can go ahead and type `ng generate component component/test` and this will create a folder for you at `src/app/components/test` with the necessary HTML, SCSS and TypeScript files. This item is automatically added to other places in Angular, so all you have to do is reference it in `src/app/app.component.html`. You have to call it `<app-test>` and anytime you create a component it will always be referenced by `<app-[name]>`.

  

You can now start the serve again and go to the browser and you will see on the page "test works!".

Since this is a static "dumb" component, we can edit it as much as we like with the server running and it will automatically refresh the browser to show your changes when you save your file.