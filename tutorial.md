This is a quick guide on how to use this engine.

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
`debuglayer()` is used for this, it displays just the layer that is specified in the `LAYER` veriable

# Displaying the whole stage

Use `refresh()` for this, this should be used to display the image a gamer should see

# Insering a single character in your stage

For this `insert(<x>, <y>, <A SIGLE CHARACTER, NOT TWO, NOT THREE, JUST ONE!1!!!1!1>)` is used
As the infuriated 
