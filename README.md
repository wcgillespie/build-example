# Build Example

This is an example starter project to help practice the following:

1. Using [Gulp 4](https://gulpjs.com) to build static assets from source files
2. Using [npm](https://www.npmjs.com) to add JavaScript libraries to the project 
3. Working with GitHub to contribute these changes in an organization

## Prerequisites

1. [Install Node and npm globally on your machine](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm). It's a good idea to also install [Node Version Manager](https://github.com/nvm-sh/nvm) as different development projects may require different versions of Node.
2. [Install Gulp 4 globally on your machine:](https://gulpjs.com/docs/en/getting-started/quick-start) `npm install --global gulp-cli`
3. Setup a Github account and fork this repository to your account [#](https://docs.github.com/en/get-started/quickstart/fork-a-repo)
4. Clone your forked repo to your machine [#](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)

## Lesson 1: Initial Build from Source
1. Navigate to the project in your terminal. Open the project in your preferred text editor and leave the terminal at the ready.
2. Open the `index.html` file in your web browser.
3. Run `npm install` in your terminal. Note this creates a `node_modules` folder, but nothing has changed yet on the page.
4. Run `gulp` in your terminal. Note a new `dist` folder is created in the project. Look at the CSS created.

### What Happened
Refresh the webpage and note how css is now present. 

Look at the `index.html` file and see how the stylesheet referenced is in the `dist` folder.

The `gulp` utility took all the materials in `src/scss/` and used it to create the `dist/css/` folder.

The way the project is configured currently, we can add any CSS or Sass code into the `_awesome.scss`, `_normal.scss`, or `_lame.scss` files and they'll all be compiled into a single css file called `app.css`.
