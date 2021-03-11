# 🖖 Vue 3 Tutorial 🖖

## Requirements

In order to use [Vue](https://vuejs.org/), we need to have [NodeJS](https://nodejs.org/en/download/) and NPM installed. Head [here](https://nodejs.org/en/download/) to download NodeJS (and NPM, which is packaged in to the download)!

If you are not on Mac or Windows, check out [here](https://nodejs.org/en/download/package-manager/) for more installation instructions.

## Lets get started

Be sure to have NodeJS installed!

You can check to make sure everything is installed properly by opening a terminal and running `node -v && npm -v` which should show two version numbers! As long as you get 2 lines of numbers, you'll be good for this lesson! If you're having problems, just Google `installing node [PLATFORM]`, like "installing node windows" and they should help you out. Google and StackOverflow is your friend!

Once you have NodeJS installed, you need to install Vue's Command Line tools. Lets get started by opening a terminal and run the install command.

```bash
# You will likely need sudo if on Linux
npm install -g @vue/cli
```

Now you have Vue's CLI installed!
```bash
# List our info, proving its installed and fully working
vue info
```

### Setting up our project

Lets get started by going in to a directory that we want to do create our project. Open a terminal where you want your project to be.

Next, we're going to run `vue create [project-name]` in order to make a vue project with all our dependencies!

We're going to specify the `--preset` flag along with the Hacksu lesson repository so you you don't have to worry about the prompts it would normally give you.

Our Vue configuration will be:
- [Vue 3](https://v3.vuejs.org/guide/introduction.html)
- [Babel](https://babeljs.io/)
- [Router](https://router.vuejs.org/guide/#html) (with History Mode)
- [Dart-Sass](https://sass-lang.com/documentation) Pre-Processor

```bash
# Create our Vue Project
vue create my-first-vue-app --preset hacksu/vue-tutorial
```

### While that's installing... what even is Vue.js?
