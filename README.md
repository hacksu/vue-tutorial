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

After waiting a moment for it to do some stuff, it should say `Listening on http://localhost:8080`. Go ahead and visit <a target="_blank" href="http://localhost:8080" >localhost:8080</a> in your browser!
