---
title: 05. Recipes
permalink: recipes.html
---

# Recipes
Our main idea was to give you strong, solid structure for your project.
At the same time we want allow you to add to and shape the project to suit your needs.

Please follow the instructions below to customize Raccoon to your needs.

## Vocabulary
### Running a command
Use your favourite terminal....
[more info needed] 
### Project root
Usually it is...[more info needed]
### Theme directory
The directory your theme files reside in.
By default it is `/public/core/themes/raccoon-theme`

## Feature missing?
### How to customize theme build process?
We use webpack for managing...
Edit... [more info needed]
### How to add Custom Post Type or Taxonomy?
Nobody wants to repeat his code. 
That is why we rely on great [Extended CPTs library by John Blackbourn](https://github.com/johnbillion/extended-cpts)

[more info needed]
### How to remove built-in jQuery 
How to remove built-in jQuery 1.x and serve 3.x without breaking the plugins
[more info needed]
### How to add Bootstrap4?
[more info needed]
### How to add Foundation5?
[more info needed]
### How to add Bourbon/Neat?
[more info needed]
### How to add React or Vue?
[more info needed]

## Feature removal
You don't like particular RaccoonWP feature? 
Please follow the recipes below to remove them from the project.

### How to remove support for Twig templates
In case you are not a fan of TWIG templating you should remove Timber plugin from your project.

Run following command in the root of your project:
```
composer remove wpackagist-plugin/timber-library
```

### How to add support for Laravel Blade templates
There are many ways to add a support for Laravel Blade templates.
In our opinion the easiest way to do so is to add [Bladerunner plugin](https://github.com/ekandreas/bladerunner) which will handle it for you.

Run following command in the root of your project:
```
composer require ekandreas/bladerunner
``` 

Afterwards navigate to the theme directory and proceed with removal of `Timber::render` function calls as well as all `[filename].twig` templates.

#### How to remove Extended CPTs
If you do not want to use Extended CPTs feature please you should remove the library from your projec dependencies.

Run the following command in the root of your project:
```
composer remove johnbillion/extended-cpts
````

[more info needed] (??)