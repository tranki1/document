# FRONTEND BOILERPLATE
This project is a highly opinionated boilerplate that can be used to quickly kickstart a new webshop. It's built on modern tools such as Gulp, Babel, and Browsersync. Using the boilerplate will help you stay productive by eliminating bikeshedding.

## Table of contents
- [➡️ Features](#%F0%9F%92%AB-features)
- [➡️ Getting started](#%E2%9E%A1%EF%B8%8F-getting-started)
  - [Set up your development environment](#set-up-your-development-environment)
  - [Creating new webshop](#creating-new-components)
  - [How to handle git](#how-to-handle-git)
  - [Quickstart](#%F0%9F%9A%80-quickstart)
  - [Contribute to code base](#contribute-to-code-base)

## ➡️ Features
- A live-reloading server with [Browsersync](https://browsersync.io/)
- Automated build process that includes, but is not limited to: SCSS compilation, JavaScript transpiling
- Source maps


## ➡️ Getting started
This boilerplate utilizes Gulp heavily to automate tasks and manage frontend dependencies. If you're new to Gulp, here's a [starter guide](https://css-tricks.com/gulp-for-beginners/).

### Set up your development environment
1. Make sure you have NodeJS installed in your machine. For detailed instructions, see:
   - [Installing Node](https://nodejs.org/en/download/package-manager/)
   - npm version 6.11.3
2. Make sure you have compass and ruby
   -ruby 2.6.5
   -compass 1.0.3
3. Navigate to your new folder and run this command to install the project-specific dependencies:
   ```
   npm install
   ```
   or `yarn`
4. Done! You can now start your development server by running `npm gulp` or `yarn gulp`. This command will start a local server, located at `http://localhost:3000`.

It's important to realize that this boilerplate has several `components`. 
-Config: Include Plus.config and Web.config
-Sass: Include all css setting
-Scripts: include all js setting

### Creating new Webshop

1. Fix file folder, proxy location on `gulpfile.js`
2. Add projectname in main Plus.config
3. Variables are located in the `components/sass/abstract/variables.scss`.You can simply change the variable need for the whole website, like brand color, max-width, font-family, font-size
4. In `components/scripts` move js component needed to include and add function on main.js
5. To minify js and css change environment to production on config.rb
The best way to get acquinted with the boilerplate is playing around with it! Try adding new components and changing old ones.

### Quickstart

1. Go to Frontend-boilerplate folder
2. Run `npm run` or `yarn`
4. Build by running `npm gulp` or `yarn gulp`

### How to handle git

Please don't merge any code changes on Frontend-boilerplate for a specific project to dev branch. All file in folder scripts/include have to be excluded from the project to prevent change in project file. Commit only your project file, DO NOT include any files in Frontend-boilerplate folder in your pull request. Create a separate brand if you really want to keep track what in the boilerplate.

### Contribute to code base 

If you have a style components or a scripts components that you use regularly and want to add to the code base. Please create a pull request on branch Feature/kimtran/Frontend-Boilerplate-for-plus and add kimtran as reviewer



