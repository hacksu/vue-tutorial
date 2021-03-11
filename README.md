# 🖖 Vue 3 Tutorial 🖖

## Requirements

In order to use [Vue](https://vuejs.org/), we need to have [NodeJS](https://nodejs.org/en/download/) and NPM installed. Head [here](https://nodejs.org/en/download/) to download NodeJS (and NPM, which is packaged in to the download)!

If you are not on Mac or Windows, check out [here](https://nodejs.org/en/download/package-manager/) for more installation instructions.

## Lets get started

Be sure to have NodeJS installed!

You can check to make sure everything is installed properly by opening a terminal and running `node -v && npm -v` which should show two version numbers! As long as you get 2 lines of numbers, you'll be good for this lesson! If you're having problems, just Google `installing node [PLATFORM]`, like "installing node windows" and they should help you out. Google and StackOverflow is your friend!

Once you have NodeJS installed, you need to install Vue's Command Line tools. Lets get started by opening a terminal and running the install command.

```bash
# You will likely need sudo if on Linux
# -g flag means global installation.
npm install -g @vue/cli
```

Now you have Vue's CLI installed!
```bash
# List our info, proving its installed and fully working
vue info
```

## Setting up our project

Lets get started by going in to a directory that we want to do create our project. Open a terminal where you want your project to be.

Next, we're going to run `vue create [project-name]` in order to make a vue project with all our dependencies!

We're going to specify the `--preset` flag along with the Hacksu lesson repository so you you don't have to worry about the prompts it would normally give you.

```bash
# Create our Vue Project
vue create my-first-vue-app --preset hacksu/vue-tutorial
```

Our Vue configuration will be:
- [Vue 3](https://v3.vuejs.org/guide/introduction.html)
- [Babel](https://babeljs.io/)
- [Router](https://router.vuejs.org/guide/#html) (with History Mode)
- [Dart-Sass](https://sass-lang.com/documentation) Pre-Processor

## While that's installing... what even is Vue.js?

Vue.js is an open-source framework used to build big, powerful websites! If you've ever heard of React and Angular; Vue is up there with them! Vue is the newest addition to the group and is currently being adopted more and more each day.

So why is this lesson about Vue and not React or Angular? Well, there's a reason why React and Angular jobs have such high salaries; they are real professional tools. Vue is designed to be a lot more casual. You can do all the same things in all 3 frameworks, but the learning curve for Vue is much easier for beginners and its a perfect stepping stone to get into React and Angular while also being the absolute perfect framework for small projects.

What are "frameworks"? Well, in the world of the JavaScript stack; there's literally a million ways to do anything. Frameworks help by implementing features developers frequently use but often implement on their own and it creates a uniform way to do things for developers. Vue, React, and Angular are used to build frontend HTML+CSS+JS applications that are really modular, clean, and super reactive and responsive! Why bother making a list of items when your framework can turn it into a single line of code!

So, hopefully your stuff is installed now. These frameworks are known for having long installation time due to all their dependencies.

## Time to start coding

Lets get our project up and running.

```bash
# Go into our project directory
cd my-first-vue-app
# Run our project with hot-relading enabled
npm run serve
```

After waiting a moment for it to do some stuff, it should say `Listening on http://localhost:8080`.

Go ahead and visit [localhost:8080](http://localhost:8080)</a> in your browser and you should see our Vue app!

## What does our project consist of?

If you open your project folder in your favorite code editor you'll see a few files and directories, but lets start out with the `src` folder.

The `src` folder is where all your source code for your app is. This is where we'll be coding.

Inside there we have a few more folders, `assets`, `components`, `router`, and `views`; along with `App.vue` and `main.js`.

- The assets folder is where we can put images and static files to be used in our app.
- The components folder is where we can put other .vue single-file components.
- The router folder is where we can put our code for `vue-router` so that our app can have different pages.
- The views folder is where we can put the entry points for our various pages.
- App.vue is the root entrypoint of our whole app
- main.js is what connects everything together.

So what does all of this mean? Well, remember when I mentioned "single-file components"? Vue works by allowing you to have a .vue file which can include HTML, JavaScript, and CSS/Sass all in one file! Single-File components can load up other single-file components which allows you to modularize your whole website!
