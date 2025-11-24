import random

def main() :
    gameWrapper()

def gameStart() :
    print("Welcome to Coin Flippers!")
    print("Would you like to start a game?")

def gameInput(response) :
    if response.casefold() == "yes".casefold() :
        print("Starting a game")
        return True
    else : 
        print("No game started")
        return False

def gameLogic() :
    print("So is it gonna be heads or tails?")
    PlayerGuess = input()
    print("So you think its " + PlayerGuess + ", eh? Well let's see...")

    randVal = random.randint(1, 6)
    # print("random value " + str(randVal))
    modVal = randVal % 2
    # print("mod value " +  str(modVal))
    if modVal == 0 :
        result = "Heads"
        if PlayerGuess.casefold() == "heads".casefold() :
            print("The coin landed on " + result + "! Congrats, you win this round!")
        else :
            print("The coin landed on " + result + "! Sorry, you lose this round.")
    else :
        result = "Tails"
        if PlayerGuess.casefold() == "tails".casefold() :
            print("The coin landed on " + result + "! Congrats, you win this round!")
        else :
            print("The coin landed on " + result + "! Sorry, you lose this round.")

def gameWrapper() :
    gameStart()
    PlayerResponse = input()
    if not gameInput(PlayerResponse) :
        return
    gameLogic()

main()