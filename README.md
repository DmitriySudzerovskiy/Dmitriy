# My first code in GidHub
import random

class Coin:
    def __init__(self):
        self.name = input("input name")
        self.win = False
        self.lost = True
        self.number = random.randint(1,21)
    def game (self, enemy):
        if self.number > enemy.number:
            print("player1=" + str(self.number))
            print("player2=" + str(enemy.number))
            print("player1 is win")
        elif self.number == enemy.number:
            print("dead heat")
        else:
            print("player1=" + str(self.number))
            print("player2=" + str(enemy.number))
            print("player2 is win")

player1 = Coin()
player2 = Coin()
