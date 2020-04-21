# diet-bulma
Some simplified bulma styles to help people coming from other css frameworks (especially bootstrap). Sass is required to compile this into a css file. This assumes you will be using node-sass and including the bulma file from node_modules. I MIGHT update and or create tutorials at my discretion, but no promises as this is mostly for my own uses (for now). Use at your own risk. Please suggest improvements.

# Setup

1. Install node-sass and bulma

If you haven't already done so in your project, create a package.json and setup node with this in terminal:

```
$ npm init
```

in terminal:

```
$ npm i -D node-sass bulma
```

# Standalone Usage (for improving Diet Bulma)

## Via Sass Command Line (automatic)

This will automatically recompile the css file from the scss (sass) file as you make changes.

in terminal:

```
$ sass --watch sass/diet-bulma.scss css/diet-bulma.css 
```


## Via npm script (manual)

This will allow you to manually run the compiler whenever you want to. 

Add this to your package.json in the "scripts" block. Like zoy:

```
"scripts": {
    "scss": "node-sass" --watch sass/diet-bulma.scss css/diet-bulma.css"
},
```

Then you can run "node scss" in terminal at will to recompile sass to css.

# Use in your project:

The instructions above are the same for if you use this in your own project, but you may need to modify the scripts or the paths to match your project's settings.

Then simply include the diet-bulma.css file into your page. Don't include bulma separately as diet bulma already does this for you.

## A little more explanation:

Diet Bulma needs to import and use styles from bulma itself. Diet Bulma overrides and merges its styles into the bulma.sass file. This is why the simplest way is to install bulma via npm and use node-sass.

Since it is reasonable to assume that many projects will use node-sass and bulma in this way, it shouldn't be much of a change to include this and start using it. If this is incorrect, please let me know by sending a PR and comments on a better way to do this and I will consider adding it. This is my first solo contribution to open-source so be nice and helpful or I will ignore your criticism. Thanks!

# WARNING
This is a work in progress. This isn't AAA software, obviously. If you can help improve this by offering better ideas or showing your thoughts in code, that would be great. If you're just going to complain, I have limited time and resources to give an eff what you think. Srsly. I am trying to contribute and help others, so don't @ me if you can't be kind.