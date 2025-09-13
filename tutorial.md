This is a quick guide on how to use this engine.

# Link Karton functions to other python files

I honestly reccomend this. Provides you a clean new python script without some random garbage at the top.

To do this first have the py file at the same location where the Karton.py file is, unless you know some more advanced black magic which will be the case 100%. Then in your py file put `from Karton import*` at the top and then go crazy.

# Creating a stage
This is the **first step** you need to do before running any other Karton command.
You can do this with `render(<width>, <height>)`
### advanced:
*this function creates a layer by the name of '#', this layer represents the width and height of the whole stage and every other layer will be created by the size of this exact layer*

# Creating a layer
You can do this with `new_layer(<Name>)`, this creates a layer at the top. So this means you should first create layers that will display at the bottom
### example
```
new_layer('background') # will appear at the back
new_layer('house') # will appear in front of the background
```
## Use `LAYER=<your layer>` to apply Karton functions to your created layers
### example
```
LAYER='background' # every Karton funcion will now apply to this layer
fill(...)
text(...)
```
## Debugging a layer
`debuglayer()` is used for this, it displays just the layer that is specified in the `LAYER` variable

# Displaying the whole stage

Use `refresh()` for this, this should be used to display the image a gamer should see

# Insering a single character in your stage

For this `insert(<x>, <y>, <A SIGLE CHARACTER, NOT TWO, NOT THREE, JUST ONE!1!!!1!1>)` is used.

As the infuriated third attrubute said, you should only put one character in the third attrubute.

Just like this: `insert(4,2,'~~') # WHY DID YOU PUT TWO CHARACTERS DAMN IT`

Sorry `insert(4,2,'~')`

**Before coninuing you need know that x and y positions are not marked like in regular game engines!**

This is how they're marked on a 5x5 stage:
```
 01234
0-----
1-----
2-----
3-----
4-----
```
# Filling

`fill (<starting x>, <starting y>, <finish x>, <finish y>, <single character>, <mode(1-2)>)` is for this

Yeah i know, that's allota attributes.

This function fills up the specified area with a specified character. **With mode set to 1 or "solid"**, it fills the whole area with your specified character without mercy towards other foreigners. **Mode set to 2 or "outline"** it draws a border in the specified area blocking out the foreigners from fresh air and freedom. **Mode set to anything else** prints you out a nice little fuck you :)

**Note: the starting x and y should be the top left corner and and finish x and y at the bottom left corner of your wanted area** otherwise instead if filling up the area i will delete your system 32 folder 

# Adding text

To add text, use `text(<x>, <y>, <max width>, <your text>)`

It adds text to your specified location by the specified width. **The x and y is where the text will start. Max width is the maximum width the text would go** before wanting another shot from the vape because oxigen tastes like shit.

Thank you for your interest towards this project!
