import random

#Ask the user for the number of NPC's 

number_npcs = int(input('Enter the number of NPCs: '))

#List of Names

name_list = ['Madoka', 'Ume', 'Reiko', 'Hitoshi', 'Nori', 'Susumu',
    'Takara', 'Orochi', 'Kiku', 'Mika', 'Aimi', 
    'Toshiko', ' Masumi', 'Takao', 'Hitomi', 'Takehiko',
    'Ayumi', 'Ameterasu', 'Chou', 'Eiji', 
    'Mieko', 'Kazumi', 'Shichiro', 'Chieko', 
    'Harumi', 'Kohaku', 'Himeru', 'Rinne', 'Niki']

#List of countries (Subject to change due to lack of originality)

country_list = ['North Country', 'South Country', 'Central Country', 'West Country', 'East Country']

#List of gender

gender_list = ['Male','Female']

# List of jobs

jobs_list = ['Merchant', 'Inn owner', 'Unemployed', 'Soldier', 'Healer', 'Pharmacist', 'Mage', 'Civil worker']

# Start loop

#Range of NPC's Generated

range_of_npcs = list(range(0, number_npcs))

#Initial Characteristic 'Values'

name = ''
age = 0
gender = ''
country = ''
model = ''
job = ''

#Generate NPC's in Loop

for i in range_of_npcs:
    name = random.choice(name_list)
    age = random.randint(6, 100)
    gender = random.choice(gender_list)
    country = random.choice(country_list)
    job = random.choice(jobs_list)
    
    if gender is 'Female' and age <= 12:
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
    
    print(f'\nName: {name} \nAge: {age} \nGender: {gender} \nModel: {model} \nCountry: {country} \nOccupation: {job} \n')


