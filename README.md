# DungeonRefactor
Refactoring for CSCD 212
added class DungeonGame

moved playAgain() from Dungeon to DungeonGame
moved battle() from Dungeon to DungeonGame
moved chooseHero from Dungeon to Hero
moved generateMonster() from Dungeon to Monster

changed chooseHero() call in main method to appropriate class - Hero.chooseHero()
changed generateMonster() call in main method to appropriate class - Monster.generateMonster()
changed battle(theHero, theMonster) call in main method to appropriate class - DungeonGame.battle(theHero, theMonster)
changted playAgain() call in main method to appropriate class - DungeonGame.playAgain()

replaced entirety of code in Keyboard to construct a static scanner named kb

replaced all referrences to previous Keyboard methods to appropriate method calls from kb
