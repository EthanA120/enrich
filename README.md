# colorich
Python module - Use ANSI formatting to color output text by hexadecimal values, RGB values or by color specific name or decorate it

Use ANSI formatting to color output text by hexadecimal values, RGB values or by color specific name or decorate
it.\
The color names and values is inspired by https://www.w3schools.com/colors/colors_names.asp and
https://github.com/jonathantneal

Functions:\
expand - Expands the colors list, extra colors will be available if this function will be executed.

enrich - Return colored and decorated font for rgb values or for hex.\
e.g. print(enrich("SeaGreen", (45, 140, 85)), "\n")\
This example will color and print the text "<span style="color: #2d8c55">SeaGreen</span>" in the rgb color of (45, 140, 85) and start a new line.

dye - Only determine the foreground color of the font but can accept a dictionary of strings with their different colors values.\
e.g. print(dye({"Periwinkle ": "periwinkle ", "Iceberg ": "Ice berg", "and ": "", "Forest green\n": "Forest green"}))\
This example will color and print the text "<span style="color: #CCCCFF">Periwinkle</span> <span style="color: #71A6D2">Iceberg</span> and <span style="color: #5FA777">Forest green</span>" with several colors - every word will be colored with the color that is writen next to it, notice that the word "and" won't be colored because no color has been assigned to it.

printr - Prints the decorated colorized text that have sent as argument.\
e.g. printr("Bold Turquoise on MediumSlateBlue", (64, 224, 208), "#7B68EE", "B", "\n")\
This example will color, decorate and print the text "<span style="color: #45B5AA; background-color: #7B68EE; font-weight: bold;">Bold Turquoise on MediumSlateBlue</span>".\
As it says, (64, 224, 208) is the text color, #7B68EE is the background color, "B" makes it bold, and \n will start a new line.

printd - Prints text that have sent as an argument in multiple colors.\
e.g. printd("Red ; red", "Slate Blue ; slateBlue", "default color ", "and; Orange Red\n; OrangeRed")\
This example will color and print the text "<span style="color: red">Red</span> <span style="color: #6A5ACD ">Slate Blue</span> default color <span style="color: #FF4500 ">and; Orange Red</span>" with several colors and eventualy will start a new line, notice that the delimeter sign ";" only apllyed as a delimeter to the last time of it's use.

show - prints all the colors and decorations name available and how it looks like.

Examples are in the bottom of the main file.


