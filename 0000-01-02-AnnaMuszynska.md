import random
from time import sleep

beginning = input("Let's create magical story together! Shall we? (Y/N): ")
if beginning == "Y":
    
    main_hero = input("First you must give a name to your main hero: ")
    gender = input("What gender is your hero? (she/he): ")
    transport = input("Mode of transportation: ")
    friend_name = input("Friend's name: ")
    positive_em = input("Positive emotion (e.g pleased, happy): ")
    negative_em = input("Negative emotion (e.g angry, sad): ")
    
    word1 = ['wand','owl','magic orb']
    word2 = ['penguins','rabbits','dragons','cats']
    word3 = ['library','bookstore','magic castle','dragon lair']
    story = f'''When {main_hero} was waiting for the {transport}, {gender} saw that {friend_name} is choosing new {random.choice(word1)}.
{gender.capitalize()} was {positive_em} that {gender} will be able to talk to old friend, but in the same moment {random.choice(word2)} 
escaped from the nearest pet shop and made chaos on the street. {main_hero} was very {negative_em} because {friend_name} was already gone. 
{gender.capitalize()} had to go to the {random.choice(word3)} alone.'''
    
    sleep(1)
    print("Story is generating!")
    print("3")
    sleep(1)
    print("2")
    sleep(1)
    print("1")
    sleep(1)
    print(story)

else:
    print("Goodbye!")
