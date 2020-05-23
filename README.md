# DungeonRefactor
Refactoring for CSCD 212

(Michael Kieburtz) Dungeon character now has a data class called DungeonCharacterStats that keeps track of all the fields that were previously in that class. 
(Michael Kieburtz) Every hero now has a specialMove instance, which represents their special move. The battleChoices() menu is no longer overridden by each Hero, and is simply defined in Hero.
(David Lopez) chooseHero() was moved into its own class called HeroFactory and from there, you can choose which character you want to be.
(David Lopez) generateMonster() was moved into its own class called MonsterFactory and with this factory, you will create a monster for the dungeon game.
(Eric Laplante) moved playAgain() from Dungeon to DungeonGame and battle() from Dungeon to DungeonGame.
(Eric Laplante and David Lopez) changed chooseHero() call in main method to appropriate class - HeroFactory.chooseHero() changed generateMonster() call in main method to appropriate class - MonsterFactory.generateMonster() changed battle(theHero, theMonster) call in main method to appropriate class  DungeonGame.battle(theHero, theMonster) change playAgain() call in main method to appropriate class - DungeonGame.playAgain().
(Eric Laplante) replaced the entirety of code in Keyboard to construct a static scanner named kb. Replaced all references to previous Keyboard methods to appropriate method calls from kb
(David Lopez) Changed the methods subtractHitPoints() to loseHealth() and attack() to normalAttack().  Changed the names of these methods because it's easy to understand what these methods do.
