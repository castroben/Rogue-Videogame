# ECE395_finalproject
This is a dungeon game created for ECE39500(Object Oriented Programming) at Purdue.
All the files necessary to run the dungeon are inside the src directory. The directory 'game' contains the bulk of the logic behind programmin the dungeon. The directory xmlfiles contains the xml files needed to initialize the dungeon. The directory asciipanel contains the code necessary to generate the window where the game is displayed. 

The game can be run from the src directory with the following line: "java game.Rogue <xmlfile>"
  
GAME COMMANDS
  'h' - move left
  
  'j' - move down
  
  'k' - move up
  
  'l' - move right
  
  'i' - display inventory
  
  'p' - pick up item. Items can only be picked up when player is standing directly on top of the item.
  
  'd' - drop item
  
  'w<inventory # for armor>' - wear an armor in inventory
  
  'T<inventory # for sword>' - yield a sword in inventory
  
  'r<inventory # for scroll>' - read a scroll in inventory

Bumping into a monster while moving around the dungeon will automatically cause the player to attack the monter and inflict some random damage within a range. This range is specified in the xml file used to run the game with the "max hit" attribute of the player. The monster will automatically strike back and inflict some random damage in a range also specified by the monter's "max hit" attribute in the xml files.


SYMBOLS
')' - sword. Yielding a sword increase the damage the player causes. The specific increase in damage can be inferred from the item's name in the xml files.
']' - armor. Wearing an armor decreases the damage done to the player.The specific increase in damage can be inferred from the item's name in the xml files.
'?' - scroll. The scrolls' functionality is specified in the xml files. Some scroll can cause the player to "hallucinate", changing the diplay of the game.
'T' - Troll (monster)
'S' - Snake (monster)
'H' - Hobgoblin (monster)

