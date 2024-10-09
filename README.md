# casio-grapher
very simple graphing function built from the ground up... in Casio BASIC

it is SLOW.

i made this more as just a challenge for me to see if i could do it.

The graph is on a fixed camera and can't be zoomed into. all plots are rounded to the nearest integer and each coordinate is one pixel.

## how to use

- functions use the variable `O` instead of `X` due to `X` being a system variable
- press up and down to navigate menus
- press EXE to select/edit items
- press F1 in the graph function menu to access the options/graph menu
- press DEL to clear a function
- press EXIT to stop graphing
- when graph is done, use left and right arrow keys to trace




## how to use but more verbose

### main menu operation
this is the main menu. here you can access the graph functions and edit them.
``` 
GRAPHER
-------------f1=Done
→Y1 20sin(10O)
 Y2 x
 Y3 x
 Y4 x
 Y5 x
```
- You are able to edit a max of 8 functions, and you can see all of them if you scroll using the up and down arrow keys.
- Functions use `O` instead of `X`

- You can press DEL to delete a function, and you will be prompted if you really want to delete it.

#### Example:
  
```
DELETE Y1?
--------------------
→NO
 YES


 
```

- If you select YES, the function will now turn into an X, meaning its deleted.

- If you input an erroneous function, the whole program will break so don't do that please thx

- You can press F1 when you are finished inputting your functions to access the **Options** menu.

### Options menu

This is your options menu, where you can choose to graph or change a very small amount of settings.

```
OPTIONS
--------------------
→GRAPH
 DISPLAY SETUP
 LINE SETUP
 BACK

```

#### GRAPH
this option will graph the functions. press EXIT to stop it prematurely, and press EXE to return to the menu.

#### DISPLAY SETUP
This is the settings for the graph display.

```
DISPLAY SETUP
--------------------
→DISPLAY AXIS?      1
 STOP ATMP AT STR   8
 DONE
 
 
```
- **DISPLAY AXIS?** is whether you want to display the X and Y axis or not.
  - valid input is 0-1
  - 1 means on, 0 means off.
  - default is 1
- **STOP ATMP AT STR** is the amount of functions you want to graph (y1-yN)
  - valid input is 1-8
  - default is 8
  
#### LINE SETUP
this is the settings for the plots in the graph. there is only one setting

```
LINE SETUP
--------------------
→LINE STEP: 1
 DONE
 

 
```

- **LINE STEP:** is the increment of `O` in the graph.
  - valid range is any real non-zero number
  - default is 1
