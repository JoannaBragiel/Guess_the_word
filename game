# Zgadnij słowo

import random

category = input("Wybierz kategorię - książka, film: ")
print(category)

list_books = ["Harry Potter", "Little women", "Hunger Games"]
list_movies = ["Joker", "Split", "Ocean 8"]

if category == "książka":
    choice = random.choice(list_books).lower()
    print(choice)
else:
    choice = random.choice(list_movies).lower()
    print(choice)

occure = {}

for i in choice:
    occure[i] = occure.get(i, 0) + 1

def user():
    
    wynik = []
    
    while(True):
        count = 0
        user_input = input("Zgadnij literę: ")
        
        if user_input in occure:
            print(("Bardzo dobrze. Litera {} zawiera się w słowie {} razy").format(user_input, occure[user_input]))
            count = count + 1
            print("Pozycja: ", choice.find(user_input))
            for i in choice:
                if i == user_input:
                    wynik.append(i)
                    print(i)
                else:
                    print("_")
            print("Zgadłeś do tej pory: ", wynik)
  
        elif len(user_input) != 1:
            print("Podaj pojedynczą literę.")
        
        else:
            user_input not in occure
            print("Nie ma tej litery w słowie. Próbuj dalej")
            continue
user()
