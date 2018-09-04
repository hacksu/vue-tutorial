# Vue Tutorial 🖖
A crash course on how to start your first Vue project!

## Overview - What is VueJS? What are we making?

VueJS is a framework to build big, powerful websites. You can actually learn Vue from its [website](https://vuejs.org/), which has great documentation and examples!

When making a larger project, you'll need to manage a ton of different files, different routes, different libraries you'll want to import, and manage data across your entire app. Here are the main tools we'll use to do that:

 - **NPM**, or **N**ode **P**ackage **M**anager, will be used to install and run different Javascript packages. Put extremely simply, this is how we can easily import tools to add to our website. We'll use this to install all our other tools - including VueJS!
 - **Webpack**, which takes all of our complicated files and links them together into one, coherent, efficient file when it gives it to the browser. This process is called **bundling**.
 - **Babel**, which takes our VueJS code and "transpiles" it into regular Javascript so browsers can read it.
 - **VueJS**, which lets us handle routing, "reactive" data, "components", and a ton of cool shortcuts! This is the main thing we'll be focusing on.
   - (If you've heard of ReactJS or AngularJS, Vue is comparable to those.)
   
## Setting up our project

We're going to use NPM to install the Vue CLI, which will let us set up a template project.

First, we're going to need NPM. To see if you have it, go to your command line, and type `npm -v`. If you get an error, you should follow this [npm installation guide](https://docs.npmjs.com/getting-started/installing-node) to get it up and running.

Next, we want to install the Vue CLI (CLI stands for **C**ommand **L**ine **I**nterface, it just means an easy way to set up a Vue project through your command line.) To install Vue CLI: 

`npm install -g @vue/cli`

Finally, we can navigate to the directory you want your Vue project, and type this to set it up: 

`vue create my-project-name`

You should see some options for setting up your project:

```
? Please pick a preset: (Use arrow keys)
❯ default (babel, eslint) 
  Manually select features 
```

Pick "manually select features", so we can look at our options! Here are the features we're going to select.

Use the arrow keys to go up and down and press `space` to toggle the options. (Enter will continue).

```
? Please pick a preset: Manually select features
? Check the features needed for your project: (Press <space> to select, <a> to tog
gle all, <i> to invert selection)
❯◉ Babel
 ◯ TypeScript
 ◯ Progressive Web App (PWA) Support
 ◉ Router
 ◉ Vuex
 ◉ CSS Pre-processors
 ◯ Linter / Formatter
 ◯ Unit Testing
 ◯ E2E Testing
```

Now, press enter! It's going to ask you a few more questions, and here's how we'll answer.
- **Y**es, we want to use history mode for the router.
- We want to use **SCSS/SASS**. (We probably won't talk about this today, but it's a really nice tool!)
- We want dedicated config files
- You can choose whether or not you want to save this. I saved this configuration as "no lint, no tests".

Finally, our project is set up! Just like your terminal says, type these two commands to get your project running:

```
cd my-project-name
npm run serve
```
