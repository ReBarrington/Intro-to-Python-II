# Python_Adventure_Game

A text-based Adventure


* The input command parser in `adv.py` allows the program to receive player input and commands to move to rooms
  in the four cardinal directions.
* Examples of valid non-directional commands are `get [ITEM_NAME]` and `drop [ITEM_NAME]` 
* Rooms are able to hold multiple items
* The player is able to carry multiple items

## Specification

The `/src` directory contains the files `adv.py`, which is where the main logic for the game lives, `room.py`, which contains the definition of the Room class, and `player.py`, which contains the definition of the Player class.


* A REPL parser in `adv.py` accepts directional commands to move the player:
  * After each move, the REPL prints the name and description of the player's current room
  * Valid commands are `n`, `s`, `e` and `w` which move the player North, South, East or West
  * The parser will print an error if the player tries to move where there is no room.

* The Room class in `room.py`: 
  * The room has `name` and `description` attributes.
  * The room also has `n_to`, `s_to`, `e_to`, and `w_to` attributes
    which point to the room in that respective direction.

* The Player class in `player.py`:
  * Players have a `name` and `current_room` attributes


* The Item class in `item.py`:
  * The item has `name` and `description` attributes.
  * This is the _base class_ for specialized item types as well.
