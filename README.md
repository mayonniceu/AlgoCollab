from random import shuffle

"""
Scrabble Game
"""
#Keeps track of the score-worth of each letter-tile.
LETTER_VALUES = {"A": 3,
                 "B": 3,
                 "C": 4,
                 "D": 2,
                 "E": 4,
                 "F": 4,
                 "G": 2,
                 "H": 4,
                 "I": 4,
                 "J": 3,
                 "K": 5,
                 "L": 3,
                 "M": 3,
                 "N": 4,
                 "O": 3,
                 "P": 3,
                 "Q": 10,
                 "R": 3,
                 "S": 4,
                 "T": 3,
                 "U": 4,
                 "V": 4,
                 "W": 4,
                 "X": 3,
                 "Y": 4,
                 "Z": 10,}
class Tile:
    """
    Class that allows for the creation of a tile. Initializes using an uppercase string of one letter,
    and an integer representing that letter's score.
    """
    def __init__(self, letter, letter_values):
        #Initializes the tile class. Takes the letter as a string, and the dictionary of letter values as arguments.
        self.letter = letter.upper()
        if self.letter in letter_values:
            self.score = letter_values[self.letter]
        else:
            self.score = 0

    def get_letter(self):
        #Returns the tile's letter (string).
        return self.letter

    def get_score(self):
        #Returns the tile's score value.
        return self.score
                 
   
                


