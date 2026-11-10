# Pocket RPG

## Repository
https://github.com/MichaelOStarr/PocketRPG

## Description
I will create a small game, with similar mechanics to a pokemon game. It will have buttons to allow for taking action, and the player will fight a cycle of random enemies.

## Features
- Main Menu
	- A main menu that allows for New Game and Load Game. These will be visual buttons that can be clicked, or by pressing N on the keyboard for new game and L on the keyboard for load game.
- Turns
	- When the game starts it is the player's turn. The player can take several actions during their turn by pressing visual buttons. After the player turn, the enemy attacks them, and it becomes the player's turn again.
- Enemy Spawn
	- When the game starts or when the previous enemy is defeated create a new enemy, its stats decided by a call to random number. The range of the random number increases with the number of defeated enemies. Stats: damage #-# health #
- Enemy Attack
	- During the enemy's turn they call for a random number based off its damage stat.
- Attack
	- An aviable action during the player's turn. Shown as a visual button and can be clicked or selected by pressing A on the keyboard. Calls for a random number based on equiped items and subtract it from the enemy's health.
- Mend
	- An aviable action during the player's turn. Shown as a visual button and can be clicked or selected by pressing M on the keyboard. Reduces the enemy's damage based off equiped items. Heal the player calling random number based off of equiped items.
- Defeating Enemy
	- When an enemy is defeated, the healing from Mend is activated. The enemy is replaced with a new enemy. A count of defeated enemies goes up. An item is created for the player and added to a list. The stats of the item are determined through a call to random number, its range dependent on the count of defeated enemies.
- Save
	- Shown as a visual button and can be clicked or seleceted by pressing S on the keyboard. The player's items, current HP, current enemy stats, current enemy health, and enemies defeated count are saved to a text file, replacing the current file if there is one
- Items
	- Shown as a visual button and can be clicked or selected by pressing I on the keyboard. Shows a visual list of the player's items, highlighting the items that are currently selected. Clicking on an item on the list replaces the currently equiped item of its respective type. Types being Weapon, Armor, and Shield. Weapon determines the random number range for Attack. Armor determines the maximum health of the player. Shield determines the healing and damage reduction of Mend.
- Load
	- A button selectable at the main menu, reads the saved file creating the necessary variables and filling lists based off of saved information.

## Challenges
- How to make visual buttons that can be clicked.
- How to make a visual that updates based off a list and can also each be clicked or selected in some way.
- How to make a save large save file.

## Outcomes
Ideal Outcome:
- The ideal outcome is having a game that can easily be navigated and is repeatable, using visual aids to enhance the experience for the player and having interactbility with the visuals.

Minimal Viable Outcome:
- Forgoing visuals for a pure text based navigation system and controls.

## Milestones

- Week 1
  1. Create an Enemy object that creates and updates an enemy.
  2. Create action for attack and mend using set numbers.

- Week 2
  1. Create an Item object that creates a random item.
  2. Create an Inventory object that manages a list of items.

- Week 3
  1. Create save file and the ability to load the save.

- Week 4
  1. Create the Main Menu.
  2. Create visuals.