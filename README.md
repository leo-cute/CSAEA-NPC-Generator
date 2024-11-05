# CSAEA-NPC-Generator

## Highlights

This program takes in a number and generates that many NPC profiles and displays their characteristics. These characteristics are the following:

* Name
* Age
* Gender
* Sprite Model (Kid, Young Male/Female, etc..)
* Country (In the context of a game)
* Job

## Overview

  Upon start, the program will ask for a integer input for the amount of NPCs the user wishes to generate. When they enter that number, the program will turn that into a range, and use it in a for loop. 
  
  For that many times, the program will choose a random name based on a list of gender-neutral names that is already provided, it will randomize an age from 6 to 50; it will also choose a gender, country, and job at random based the lists for each category that are provided.
  
  Based on the gender and age, the program will run through a series of conditional statements in order to choose the sprite model that best fits both characteristics. For example, if the character is 10 years old, it will assign it a 'Kid' sprite model, regardless of gender. If the character is 28 years old, and is female, the program will assign it a 'Tall Female' model, as the program assigns such to all females over 25 years of age. The program runs through similar series of conditionals for other ages. 
  
  At the end of the loop, the program will print the profile of the NPC, with each characteristic on a separate line. This goes on for however many NPCs the user asked the program to generate.

## Code Sample

This is how the program decides what sprite model to assign the NPC, based on the already set age and gender.

```
    if age <= 12:
        model = 'Kid'
    elif gender is 'Female' and 12 < age <= 25:
        model = 'Young Female'
    elif gender is 'Female' and 25 < age:
        model = 'Tall Female'
    elif gender is 'Male' and age <= 12:
        model = 'Kid'
    elif gender is 'Male' and 12 < age <= 25:
        model = 'Young Male'
    elif gender is 'Male' and 25 < age:
        model = 'Tall Male'
```

This is the information displayed for each NPC.

```
print(f'\nName: {name} \nAge: {age} \nGender: {gender} \nModel: {model} \nCountry: {country} \nOccupation: {job} \n')

```

An example of what one NPC profile would look like in the output would look like this:

```
Name: Tayo
Age: 16
Gender: Female
Model: Young Female
Country: North Country
Occupation: Inn owner
```
