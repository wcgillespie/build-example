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

## Lesson 2: Play with Git

### Ignored files
In the earlier steps we created a `node_modules` directory with npm and a `dist` directory with Gulp.

1. Look at the `.gitignore` file in the project. See which directories are not being tracked by git?
2. In your terminal run the command `git status` and read the output.
3. Add some new Sass/CSS to one of the files in the `src/css/` directory.
4. Note on the webpage the change hasn't taken effect.
5. In the terminal, run `gulp` to build the changes. Refresh the webpage and note the effect.
6. In the terminal, run `git status` and note output: we're tracking `src/` but not `dist/`.

### Work in a branch in your GitHub repo

In the terminal, run these commands:

`git branch feature/styles`

`git checkout feature/styles`

`git add .`

`git commit -m "Adding new styles"`

`git push`

Checkout your forked repository on GitHub.com now. Your branch is visible.

### Manage the project in GitHub

1. Create a Pull Request (PR) of your `feature/styles` branch into the `main` branch of your repo
2. Merge the PR
3. In your terminal, run `git checkout main`
4. Run `git pull`
5. Run `git log`

The new styles added to `main` were "truth" in GitHub first. We made our local machine catch up - even though we started those style changes on our machine. This process can expand to many developers contributing changes nicely.