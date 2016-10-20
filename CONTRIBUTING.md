# Installation
          
```sh
git clone https://github.com/JClerc/GreenSpot.git
cd GreenSpot
git checkout develop
npm install
```

# Working with Gulp

If you have Gulp installed globally:
```
gulp
```

And if you haven't:
```
npm run gulp
```

# Guidelines

### General

Indentation is made with 4 spaces.

### CSS

We are using [SCSS](http://sass-lang.com/) for making our styles, and [BEM](https://en.bem.info/) for naming conventions.

### JavaScript

ES6 is used (and converted to ES5 using Babel) in our project. We use the general coding conventions, as defined [here](http://www.w3schools.com/js/js_conventions.asp).

# Merging branches

Branches have to be merged in squash mode, with version as commit message.

```sh
# Move to master
git checkout master
# Merge without history, and discard changes in master
git merge develop --squash -X theirs
# Commit with version number
git commit -m "Version X.X.X"
```
