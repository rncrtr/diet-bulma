# diet-bulma
Some simplified bulma styles to help people coming from other css frameworks (especially bootstrap). Sass is required to compile this into a css file. This assumes you will be using node-sass and including the bulma file from node_modules. I MIGHT update and or create tutorials at my discretion, but no promises as this is mostly for my own uses (for now). Use at your own risk. Please suggest improvements.

# Setup

1. Install node-sass and bulma

If you haven't already, create a package.json and setup node with this:

in terminal:

```
$ npm init
```

in terminal:

```
$ npm i -D node-sass bulma
```

# Usage

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
    "scss": "node-sass" --watch assets/scss -o assets/css"
},
```

Then you can run "node scss" in terminal at will to recompile sass to css.