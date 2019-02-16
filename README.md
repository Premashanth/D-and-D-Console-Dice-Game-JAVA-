Design and Implement a character generator for a game. It should have the following specifications:
•	The program should ask for a Level.
•	The program should offer a selection of Classes or Professions to choose from and accept a choice.
•	The program should then offer a variety of methods of generating the attributes
o	The attributes should be: Str, Dex, Con, Int, Wis, and Cha
o	The program should offer a selection of methods of generation such as:
	Entering the attributes directly
	Roll 4d6 and discard the lowest value.
	Roll 4d6 and discard the lowest value and if the attribute is 16 or higher, add the value of an additional 1d6.
	Roll Method IX:
•	Each class should weight each attribute from most to least important. In Method IX, the most important attribute rolls 9d6 and keeps the highest 3. The second most important rolls 8d6, keeping the highest 3. This follows in this pattern of 7d6, then 6d6, then 5d6 and finally 4d6 for the least important. 
•	Each attribute confers a bonus or penalty. Through the Workshops you should have deduced that the pattern for the bonuses follows the formula y = (x/2)-5.
•	Once the attributes have been rolled, calculate the hitpoints for the character. This should be the total value of 1 hitdice rolled and combined with the Con bonus (either positive or negative) for each level. If the Con bonus is negative, your program should ensure that the minimum value for every level is 1. (You cannot have 0 or a negative number for any level).
•	Present the values generated as one set and either allow the user to accept or discard (and regenerate) the attributes. The program should remember the values entered for Level and Class/Profession
•	Once a set of attributes has been accepted, you should allow the user to select skills.
o	Each Class/Profession should get a different number of skill-points per level.
o	The number of skill-points a character has should be the number of skill-points the Class/Profession grants combined with the Int bonus. If the Int bonus is negative this should be a minimum of 1 skill-point for each level. The first level should get 4 times the number of skill-points but only the first level!
o	Each skill should have a maximum number of skill-points allocated to it of Level + 3.
•	Once all skill-points have been spent, calculate the following:
o	Base Attack Bonus (BAB). This is something determined by Class/Profession (as in there should be a difference between classes) and should be one of the following:
	For combat orientated Classes/Professions: BAB = Level 
	Classes/Professions you think are average at combat: BAB = (Level*3)/4 
	Classes/Professions you think are combat adverse: BAB = Level/2 
o	Combat and Damage should be BAB + Str bonus and Str bonus respectively. 
•	Ask for and accept a character name
•	Display all the information neatly. The character name and level, all attributes and bonuses, hit-points, base attack bonus, combat and damage bonus and all selected skills (with number of skill points).
•	Offer the option of saving the character to a file (and actually save it if requested) before making a new character or quitting.
•	Classes/Professions and Skills should be stored in files and read in at runtime. 
