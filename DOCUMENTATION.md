# Changing the Preloaded Snap Code

The Snap code that is preloaded when you start the program cannot be changed through the website due to certain functionalities being disabled. To change the code, go to the "src" folder and open xmlfile.js. This file contains a single variable named xmlfile that holds a string of XML code (which is the format that Snap code is saved in). Replace this XML code with your XML code (make sure to keep it as a string), save the file, and refresh the HTML.

# Changes Made to the Original Snap Code

Here is a rough list of the changes made to the original Snap repository. The javascript file noted at the beginning of each line is the file that has been modified, followed by what was changed in that file:

- byob.js: commented line 1255 to disable editing blocks
- gui.js: commented lines 2482 - 2484 and uncomment 2485 to disable switching sprites by clicking on their icons
- object.js: commented blocks from line 2357 to get rid of blocks
- object.js: commented 136-147 to get rid of block tabs
- gui.js: commented lines 1762, 1785, 1815 to get rid of new sprites, paints, and camera buttons
- gui.js: commented function SpriteIconMorph.prototype.userMenu except for var def and return to disable right-clicking sprites
- gui.js: commented SpriteIconMorph.prototype.duplicateSprite and SpriteIconMorph.prototype.removeSprite to prevent altering sprites
- gui.js: commented line 1544 to disable dragging on stage
- gui.js: commented lines 1606 and 1622 to get rid of costumes and sounds tabs
- gui.js: commented lines 1078, 1048, and 1025 to get rid of cloud, settings, and project buttons
- gui.js: commented line 3200 to get rid of Snap logo menu
- gui.js: commented line 1505 to get rid of renaming
- gui.js: commented line 1467 to get rid of transformations
- gui.js: commented line 1486 to get rid of sprite icon
- byob.js: commented lines 1957-1966 and changed line 1716 to false to default to creating local blocks
- gui.js: commented lines 1860 and 1864 to get rid of the sprite menu at the bottom-right of the website
- objects.js: commented line 6173 to disable double-clicking sprites on stage
- byob.js: changed line 3886 to false and comment lines 3903-3912 to default to creating local variables
- objects.js: changed 2686 to true to enable JS by default
- threads.js: commented line 1236 to disable JS error message
- object.js: changed line 3050 to false to disable hiding primitives (aka default blocks)
- object.js: commented lines 3039 to 3049 to disable finding blocks

Please note that the line numbers may not be 100% accurate due to the line numbers correlating to a previous version of Snap. However, the correct line number should be within 50 lines of code from the given number.