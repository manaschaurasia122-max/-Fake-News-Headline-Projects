#1- import the random module
import random

#2- create subjects list
subjects=[
    "Shahrukh Khan",
    "Salman Khan",
    "Aamir Khan",
    "Virat Kohli",
    "Nirmala Sitharaman",
    "A Mumbai Cat",
    "A Group of Monkeys",
    "Prime Minister Narendra Modi",
    "Auto Rickshaw Drivers from delhi",
]

actions=[
    "launched",
    "Cancels",
    "dances with",
    "eats",
    "sings with",
    "declares war on",
    "gives a speech to",
    "orders",
    "celebrates"   
]

places_or_things=[
    "at red fort",
    "in Mumbai local train",
    "a plote of samosa",
    "inside parliment house",
    "at a cricket stadium",
    "during IPL Match",
    "at Ganga Ghat",
    "in a restaurant",
    "at India Gate" 
]

#3-start the headline generation loop
while True:
    subject=random.choice(subjects)
    action=random.choice(actions)
    place_or_thing=random.choice(places_or_things)

  headline=f"BREAKING NEWS: {subject} {action} {place_or_thing}!"
    print("\n"+headline)


   user_input=input("\n Do you want another hedline? (yes/no): ").strip()
    if user_input=="no":
        break


#print goodbye message
print("\nThank you for using the Fake News Headline Generator.Have a Fun day")

