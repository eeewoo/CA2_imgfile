# Starter Repository for Assignment
You are required to build your folder structures for your project.

## Folder Structure
```json
/BED-CA2-P2331308-DIT_FT_1B_05
    ├── data
    │   ├── enemy.csv
    │   └── spell.csv
    ├── node_modules
    ├── public
    │   ├── css
    │   │   └── carousel.css
    │   │   └── color.css
    │   │   └── style.css   
    │   ├── images 
    │   │   └── carousel-images
    │   │   └── class-images
    │   │   └── enemy-images   
    │   │   └── general-images   
    │   │   └── spell-images   
    │   └── js
    │      └── getClassById.js
    │      └── getCombatSessionById.js
    │      └── getCompletionById.js
    │      └── getCurrentURL.js
    │      └── getPlayerSaveFile.js
    │      └── getSingleEnemyInfo.js
    │      └── getSinglePlayerInfo.js
    │      └── getSpellbookCollection.js
    │      └── leaderboardGraph.js
    │      └── loginUser.js
    │      └── postChallenge.js
    │      └── postChallengeRevision.js
    │      └── postCombatRef.js
    │      └── postSingleFitnessCompletion.js 
    │      └── postSpellbooks.js
    │      └── postSpellPurchase.js
    │      └── queryCmds.js
    │      └── registerUser.js
    │      └── showAllClasses.js
    │      └── showAllCombatRef.js
    │      └── showAllEnemy.js
    │      └── showAllFitness.js
    │      └── showAllFitnessRevision.js
    │      └── showAllPlayers.js
    │      └── showAllSpellbooks.js
    │      └── showAllSpells.js
    │      └── showAllUsers.js
    │      └── skillpointsStats.js
    │      └── userNavbarToggle.js
    │      └── utils.js
    ├──  classes.html
    ├──  combat.html
    ├──  enemy.html
    ├──  fitness.html
    ├──  index.html
    ├──  leaderboard.html
    ├──  login.html
    ├──  players.html
    ├──  profile.html
    ├──  register.html
    ├──  singleClassInfo.html
    ├──  singleCombatInfo.html
    ├──  singleEnemyInfo.html
    ├──  singleFitnessInfo.html
    ├──  singlePlayerInfo.html
    ├──  singleSpellbookInfo.html
    ├──  singleUserInfo.html
    ├──  spellbooks.html
    ├──  spells.html
    ├──  users.html
    ├── src
    │   ├── configs
    │   │   └── createSchema.js
    │   │   └── createUsers.js
    │   │   └── initTables.js
    │   ├── controllers
    │   │   ├── challengeController.js
    │   │   ├── classController.js
    │   │   ├── combatrefController.js
    │   │   ├── enemyController.js
    │   │   ├── leaderboardController.js
    │   │   ├── playerController.js
    │   │   ├── reviewController.js
    │   │   ├── spellbooksController.js
    │   │   ├── spellController.js
    │   │   └── userController.js
    │   ├── middlewares
    │   │   ├── bcryptMiddleware.js
    │   │   └── jwtMiddleware.js
    │   ├── models
    │   │   ├── challengeModel.js
    │   │   ├── classModel.js
    │   │   ├── combatrefModel.js
    │   │   ├── enemyModel.js
    │   │   ├── leaderboardModel.js
    │   │   ├── playerModel.js
    │   │   ├── playerModel.js
    │   │   ├── spellbooksModel.js
    │   │   ├── spellModel.js
    │   │   └── userModel.js
    │   ├── routes
    │   │   ├── challengeRoutes.js
    │   │   ├── classRoutes.js
    │   │   ├── combatrefRoutes.js
    │   │   ├── enemyRoutes.js
    │   │   ├── leaderboardRoutes.js
    │   │   ├── mainRoutes.js
    │   │   ├── playerRoutes.js
    │   │   ├── reviewRoutes.js
    │   │   ├── spellbooksRoutes.js
    │   │   ├── spellRoutes.js
    │   │   └── userRoutes.js
    │   └── services
    │       └── db.js
    ├── app.js
    ├── .env
    ├── .env.local
    ├── .env.production.local
    ├── .gitignore
    ├── index.js
    ├── package-lock.json
    ├── package.json
    └── README.md
```

## Installation Of Required Modules Dependencies and Set Up
0: Clone Git Repo Link, make sure it is correct: (CA1)
https://github.com/ST0503-BED/bed-ca1-dramatictan 

0.1: Clone Git Repo Link, make sure it is correct: (CA2)
https://github.com/ST0503-BED/bed-ca2-dramatictan

1: npm init (if you do not see package.json in the file, but most likely have)

2: npm i (installing the package into package.json and node module)

3: npm i nodemon express mysql2 dotenv

3.2: npm install jsonwebtoken bcrypt

4: set up .env file (here is my .env file for reference)
```json
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=root
DB_DATABASE=bed_ca1

JWT_SECRET_KEY=your-secret-key
JWT_EXPIRES_IN=15m
JWT_ALGORITHM=HS256
```
5: Run this script on terminal to load the users with their hashed password
```json
node src/configs/createUsers.js  
```

6: Run this script on terminal to load data 
```json
npm run init_tables   
```

7: npm run dev (to run website)

### If missing modules are detected, please install the following modules

1: npm i nodemon express mysql2 dotenv

2: npm i 

3: npm install jsonwebtoken bcrypt

### If error still persist, please type this in to package.json top codes. But it should be present in the code.

"init_tables": "node src/configs/createSchema.js && node src/configs/initTables.js",
"start": "node index.js",
"dev": "nodemon index.js"

# CA2 (PART 2)
# How to Run Application Website
## Website URL once npm run dev 
```json
http://localhost:3010/index.html


Youtube Demo Video Link: https://www.youtube.com/watch?v=pxLY_9ewUFQ
```

## Navigating through the website:
1: Register to make your own account

2: Login with your account details

3: Complete some challenges in the challenge page to earn skillpoints. Or create your own challenges
```json
Press the Complete Challenge button on one of the challenge boxes 

Write notes
Select option box either completed or not completed
```

4: Post a review about the challenges 
```json
Fill in form to post your review

Enter your own user ID
Rate from 1 to 5 stars
Enter your reviews

Press Submit button to post
```

5: Create a spellbook to collect spells. User can make more than one spellbook
```json
Fill in spellbook creation form 

Enter your user ID so you can own that spellbook
Enter spellbook name

Press Create button to post
```

6: Go to Class page to buy spells. The Class page have unique classes which teaches different types of spells. For example, a Charms Class would teach only Charm Spells.
```json
Enter a class

Enter the spell ID of the spell you want to buy
Enter the type (Must be the same input as Class)
Enter the Class name (Must be the class you are in right now)
Enter Spellbooks ID (to take the purchased spell into inside that spellbook)

NOTE:
Type and Class Name input must be the SAME
Spellbooks ID and Spell ID must exist 
```

7: Create your own player character
```json
Player Creation Form

Enter player name
Enter your user id to link Player to you
Enter spellbook id to link to Player

NOTE:
User ID and Spellbook ID must exist to work.
```

8: Combat Form
```json
Battle Request Invitation Card

Enter player ID
Enter enemy ID

NOTE:
Player and enemy ID must exist to work
```

9: Combat System
Player already have the spellbook to use.

Spellbook consist of the spells you purchased

Enemy have different stats that makes it easier or harder such as:
- Health 
- Type of spells it uses (some enemies have or do not have, which is called 'Specialist')
- Damage Range (10-50 means enemy can use spells that deal 10 to 50 damage)
- Heal Range (10-50 means enemy can heal 10 to 50 health)

HOW TO PLAY:
```json
Press attack button to deal damage
Press heal button to heal up
Enemy can either attack or heal randomly as well when you do actions
```

# CA1 (PART 1)
# How To Run Application
## 1: POST /users
Create a new user by providing their username in the request body. Upon successful
creation, the response should include the newly generated user_id.
### Example Request Body
``` json
{
    "username": "socuser321"
}
```
### Example Response
``` json
{
    "user_id": 1,
    "username": "socuser321",
    "skillpoints": 0
}
```
Status Code: 201 Created

### Error Handling:
If the provided username is already associated with another user, return 409 Conflict.

If the request body is missing username , return 400 Bad Request.

## 2: GET /users
Retrieve a list of all users with their respective `user_id`, `username`, and `skillpoints`.
### Example Response
```json
[
    {
        "user_id": 1,
        "username": "socuser321",
        "skillpoints": 0
    },
    {
        "user_id": 2,
        "username": "fitnessKing",
        "skillpoints": 0
    }
]
```
Status Code: 200 OK

### Error Handling:
If the requested user_id does not exist, return 404 Not Found.

If the provided username is already associated with another user, return 409
Conflict

## 3: PUT /users/{user_id}
Update user details by providing `user_id` in the URL and updating `username` in the request body.

### Example Request Body
```json
{
    "username": "superSOC",
    "skillpoints": 100
}
```
### Example Response
``` json
{
    "user_id": 1,
    "username": "superSOC",
    "skillpoints ": 100
}
```
Status Code: 200 OK

### Error Handling:
If the requested user_id does not exist, return 404 Not Found

If the provided username is already associated with another user, return 409 Conflict

## 4: POST /challenges
Create a new fitness challenge by providing user_id , challenge and skillpoints in the
request body. Upon successful creation, the response should include the newly
generated challenge_id, the user_id will be inserted as creator_id .

### Example Request Body:
``` json
{
    "challenge": "Complete 2.4km within 15 minutes",
    "user_id": 1,
    "skillpoints": 50
}
```
### Example Response:
``` json
{
    "challenge _id": 1,
    "challenge": "Complete 2.4km within 15 minutes",
    "creator_id": 1,
    "skillpoints": 50
}
```
Status Code: 201 Created

### Error Handling:
If the request body is missing challenge, user_id , or skillpoints return 400 Bad
Request.

## 5: GET /challenges
Retrieve a list of all challenges with their respective challenge_id , challenge , creator_id
and skillpoints

### Example Response
```json
[
    {
    "challenge _id": 1,
    "challenge ": "Complete 2.4km within 15 minutes",
    "creator_id": 1,
    "skillpoints": 50
    },
    {
    "challenge _id": 2,
    "challenge": "Cycle around the island for at least 50km",
    "creator_id": 1,
    "skillpoints": 100
    }
]
```
Status Code: 200 OK

## 6: PUT /challenges/{challenge_id}
Update challenge details by providing challenge_id in the URL and updating the fitness
challenge in the request body. Do ensure that the user trying to update the challenge is
the same as the creater.
### Example Request Body
```json
{
    "user_id": 1,
    "challenge": "Complete 2.4km within 12 minutes",
    "skillpoints": 75
}
```
### Example Response:
```json
{
    "challenge _id": 1,
    "challenge": "Complete 2.4km within 12 minutes",
    "creator_id": 1,
    "skillpoints": 75
}
```
Status Code: 200 OK

### Error Handling:
If the requested challenge_id does not exist, return 404 Not Found.

If the request body is missing challenge, skillpoints or user_id, return 400 Bad
Request.

If creator_id is different from the user_id, return 403 Forbidden due to not
correct creator.

## 7: DELETE /challenges/{challenges_id}
Delete a challenge by providing its challenge_id . The challenges's associated user
completions, if any, should also be deleted.

No Response Body

Status Code: 204 No Content

### Error Handling:
If the requested challenge_id does not exist, return 404 Not Found.

## 8: POST /challenges/{challenge_id}
Create an completion record from a user (marking a challenge complete) by providing
challenge_id in URL parameter and user_id, completed , creation_date, and notes in
the request body

### Example Request Body
```json
{
    "user_id": 1,
    "completed": true,
    "creation_date": "2024-11-30",
    "notes": "A fitter me!"
}
```
### Example Response
```json
{
    "complete_id": 1,
    "challenge_id": 1,
    "user_id": 1,
    "completed": true,
    "creation_date": "2024-11-30",
    "notes": "A fitter me!"
}
```
Status Code: 201 Created

### Error Handling:
If the requested user_id or challenge_id does not exist, return 404 Not Found.

If the request body is missing creation_date , return 400 Bad Request.

Additional Requirements:
Upon successfully completing a challenge question, the user will receive the
amount of skillpoints awarded to that challenge. Award 5 skillpoints if
challenge was attempted but completed is indicated as false.

## 9: GET /challenges/{challenge_id}/
Retrieve list of participants who attempted a particular challenge by providing its
challenge_id. The response should include user_id, creation_date, completed, and
notes.
### Example Response:
```json
[{
    "user_id": 2,
    "completed": true,
    "creation_date": "2024-11-30",
    "notes": "A fitter me!"
    },
    {
    "user_id": 3,
    "completed": false,
    "creation_date" :"2024-10-30",
    "notes": "I don’t like this challenge"
}]
```
Status Code: 200 OK

### Error Handling:
If the requested challenge_id does not have any user attempts, return 404 Not
Found.

# Section B: Infuse Gamification
### Theme Idea: Magicial Academia 
My Endpoint Ideas include:

1: Created endpoints for managing the inventory of magicial spells.

2: Created endpoints for a shop system to purchase spells using skillpoints.

3: Created endpoints for character customization, allowing players to choose which abilites and powers they want.

4: Created endpoints for accepting enemy battles, with attacking and healing, with rewards if player win.

## How Does It Work:
1: Users can start completing challenges to earn skillpoints as a form of currency

2: Users can go to Classes, to learn different spells with different types, attack, healing and abilities.

3: Users after purchasing spells can store their selected spells in a spellbook.

4: Users can set up their player persona and link their spellbook to that player. Users can create multiple persons, with different spellbooks.

5: Players can fight against an Enemy with various difficulities and stats, such as higher health, specalists, and attack patterns.

6: Users can go to leaderboards as a form of social interaction.

# Spell 
## 1: POST /spell
Create a spell with the following data in the request body, spellName, type1, spellInfo, damage, heal and effect. spellInfo and effect is optional.
### Example Request Body
```json
{
    "spellName": "Iuvenaleaqua",
    "type1": "Charms",
    "spellInfo": "A simple cast of fresh water that provide a soothing healing relieve to injuries.",
    "damage": 0,
    "heal": 20,
}
```
### Response Body
```json
{
    "spell_id": 1,
    "spellName": "Iuvenaleaqua",
    "type1": "Charms",
    "spellInfo": "A simple cast of fresh water that provide a soothing healing relieve to injuries.",
    "damage": 0,
    "heal": 20
}
```
Status Code: 201 Created
### Error Handling
If the request body is missing spellName, type1, damage and heal, return 400 Bad Request.

If the request body damage or heal value is not between 10 to 200, return 400 Bad Request

If the request body have the same spellName, return 409 Conflict.

##  2: GET /spell
Retrieve a list of spells with their respective spell_id, spellName, type1, spellInfo, damage, heal and effect
### Response Body
```json
[
    {
        "spell_id": 1,
        "spellname": "Iuvenaleaqua",
        "type1": "Charms",
        "spellinfo": "A simple cast of fresh water that provide a soothing healing relieve to injuries.",
        "damage": 0,
        "heal": 20,
        "effect": null
    },
    {
        "spell_id": 2,
        "spellname": "Paramentis",
        "type1": "Charms",
        "spellinfo": "A simple reliable barrier charm to protect the cast from any offensive spells. However, the barrier may crack if the offensive spell is more destructive.",
        "damage": 0,
        "heal": 30,
        "effect": null
    },
    {
        "spell_id": 3,
        "spellname": "Eh-Ka-Polsion",
        "type1": "Charms",
        "spellinfo": "Unleash a destructive explosive spell, shredding anything in it's path.",
        "damage": 50,
        "heal": 0,
        "effect": null
    },
    {
        "spell_id": 4,
        "spellname": "Atom Understanding",
        "type1": "Charms",
        "spellinfo": "Understand how every elements are aligned based on their properties, bonding and particle numbers, allowing you to create anything you want",
        "damage": 70,
        "heal": 30,
        "effect": null
    },
    {
        "spell_id": 5,
        "spellname": "Umbra Tenebris",
        "type1": "Dark Arts",
        "spellinfo": "Wrap the victim's heart with dark tendrils, locking and tightening their heart from pumping blood if they even move a single inch.",
        "damage": 20,
        "heal": 0,
        "effect": "poison"
    }
]
```
Status Code: 200 OK

## 3: PUT /spell/{spell_id}
Update spells details by providing `spell_id` in the URL and updating spellName, type1, spellInfo, damage, heal and effect in the request body. 

spellInfo and effect is optional.
### Example Request Body
```json
    {
        "spellName": "Paramentiss",
        "type1": "Charms",
        "spellInfo": "A simple reliable barrier charm to protect the cast from any offensive spells. However, the barrier may crack if the offensive spell is more destructive.",
        "damage": 0,
        "heal": 30,
        "effect": "defense"
    }
```
### Response Body
```json
{
    "spell_id": 2,
    "spellName": "Paramentiss",
    "type1": "Charms",
    "spellInfo": "A simple reliable barrier charm to protect the cast from any offensive spells. However, the barrier may crack if the offensive spell is more destructive.",
    "damage": 0,
    "heal": 30,
    "effect": "defense"
}
```
Status Code: 200 OK

### Error Handling:
If the request body have the same spellName, return 409 Conflict.

If spell id does not exist, return 404 Not Found

## 4: DELETE /spell/{spell_id}
Delete a spell by providing its spell_id . The spell's associated data, if any, should also be deleted.

No Response Body

Status Code: 204 No Content

### Error Handling:
If the requested spell_id does not exist, return 404 Not Found.

# Spellbooks 
## 1: POST /spellbooks
Create a spellbook with the following data in the request body, spellbooks_name and userSpellbooks_id. userSpellbooks_id is the same as user_id in User Table, to show that this spellbook belongs to user.
### Example Request Body
```json
{
    "spellbooks_name": "Guan Ying First Spellbook",
    "userSpellbooks_id": 3
}
```
### Response Body
```json
{
    "userSpellbooks_id": 3,
    "spellbooks_name": "Guan Ying First Spellbook"
}
```
Status Code: 201 Created
### Error Handling:
If the request body is missing data, return 400 Bad Request.

## 2: GET /spellbooks/{username}
Retrieve a list of spellbooks created by the username with their respective spellbooks_id, spellbooks_name, userSpellbooks_id, owner_id and ownerUsername

Note: userSpellbooks_id and owner_id is the same as user id in User Table. I did that to check if both values are the same to confirm. ownerUsername is the same as the username in User table. First method by username

### Response Body
```json
[
    {
        "spellbooks_id": 1,
        "spellbooks_name": "Guan Ying First Spellbook",
        "userSpellbooks_id": 3,
        "owner_id": 3,
        "ownerUsername": "guan ying"
    },
    {
        "spellbooks_id": 2,
        "spellbooks_name": "Guan Ying Second Spellbook",
        "userSpellbooks_id": 3,
        "owner_id": 3,
        "ownerUsername": "guan ying"
    }
]
```
### Error Handling:
If the requested username does not exist, return 404 Not Found.

## 3: GET /spellbooks/userId/{userSpellbooks_id}
Retrieve a list of spellbooks created by the username with their respective spellbooks_id, spellbooks_name, userSpellbooks_id, owner_id and ownerUsername. Second method by userSpellbooks_id.

### Response Body 
```json
[
    {
        "spellbooks_id": 1,
        "spellbooks_name": "Guan Ying First Spellbook",
        "userSpellbooks_id": 3,
        "ownerUsername": "guan ying"
    },
    {
        "spellbooks_id": 2,
        "spellbooks_name": "Guan Ying Second Spellbook",
        "userSpellbooks_id": 3,
        "ownerUsername": "guan ying"
    }
]
```
### Error Handling:
If the requested username does not exist, return 404 Not Found.

## 4: DELETE /spellbooks/{userID}/{userSpellbooks_id}/spellbooksID/{spellbooks_id}
Delete a spell by providing its userID, (userID is the same as user_id from User table), userSpellbooks_id and spellbooks_id.

No Response Body

Status Code: 204 No Content

### Error Handling:
If the requested spellbooks_id does not exist or does not belong to user, return 404 Not Found.

## 5: PUT /spellbooks/{userSpellbooks_id}/userId{spellbooks_id}/edit
Update spells details by providing `userSpellbooks_id` which is the id of owner of the spellbook and spellbooks_id in the URL and updating spellbooks_name.
### Example Request Body
```json
{
    "spellbooks_name": "Updated Spellbooks"
}
```
### Response Body
```json
{
    "spellbooks_id": 2,
    "spellbooks_name": "Updated Spellbooks"
}
```
Status Code: 200 OK
### Error Handling:
If the request body is missing spellbooks_name, return 400 Bad Request.

If the requested spellbooks_id does not exist or does not belong to user, return 404 Not Found.

## 6: GET /enter/userID/{userSpellbooks_id}/spellbooksID/{spellbooks_id}
Retrieve a list of spells inside that spellbook id created by the user, spellbooks_name, userSpellbooks_id, owner_id and ownerUsername. Second method by userSpellbooks_id.
### Response Body
```json
{
    "message": "Spells retrieved successfully!",
    "data": [
        {
            "ownerUsername": "guan ying",
            "spellbooks_name": "Updated Spellbooks",
            "spellbooks_id": 2,
            "spell_id": 5,
            "name": "Umbra Tenebris",
            "type": "Dark Arts",
            "ability": "Wrap the victim's heart with dark tendrils, locking and tightening their heart from pumping blood if they even move a single inch.",
            "damage": 20,
            "heal": 0,
            "effect": "poison"
        },
        {
            "ownerUsername": "guan ying",
            "spellbooks_name": "Updated Spellbooks",
            "spellbooks_id": 2,
            "spell_id": 6,
            "name": "Shou Ling Tong",
            "type": "Dark Arts",
            "ability": "A punishing spell created to targets the nerves in the victim's hand, sending waves of excruciating pain every time they attempt to touch anything or casting a spell.",
            "damage": 30,
            "heal": 0,
            "effect": "poison"
        },
        {
            "ownerUsername": "guan ying",
            "spellbooks_name": "Updated Spellbooks",
            "spellbooks_id": 2,
            "spell_id": 7,
            "name": "Sanguinem Blood",
            "type": "Dark Arts",
            "ability": "User is able to manuplate it's own blood into various forms as weapons or armor, bombs and increasing blood flow..",
            "damage": 30,
            "heal": 30,
            "effect": null
        },
        {
            "ownerUsername": "guan ying",
            "spellbooks_name": "Updated Spellbooks",
            "spellbooks_id": 2,
            "spell_id": 1,
            "name": "Iuvenaleaqua",
            "type": "Charms",
            "ability": "A simple cast of fresh water that provide a soothing healing relieve to injuries.",
            "damage": 0,
            "heal": 20,
            "effect": null
        },
        {
            "ownerUsername": "guan ying",
            "spellbooks_name": "Updated Spellbooks",
            "spellbooks_id": 2,
            "spell_id": 17,
            "name": "Thousand Petal Dance",
            "type": "Elemental",
            "ability": "Summons a storm of razor-sharp petals that swirl gracefully around the caster, cutting enemies in range.",
            "damage": 60,
            "heal": 60,
            "effect": null
        },
        {
            "ownerUsername": "guan ying",
            "spellbooks_name": "Updated Spellbooks",
            "spellbooks_id": 2,
            "spell_id": 16,
            "name": "Blossoming Love",
            "type": "Elemental",
            "ability": "A gentle spell that summons radiant flowers to bloom around the target, soothing their pain and healing their wounds with a warm, comforting energy.",
            "damage": 0,
            "heal": 80,
            "effect": null
        }
    ]
}
```
### Error Handling:
If the spellbook for the given user or spellbooks_id does not exist, return 404 Not Found.

# Class 
## 1: POST /class
Create a class with the following data in the request body, className and classDescription and skillpointsCost. 
### Example Request Body
```json
{
    "className": "Charms",
    "classDescription": "This class room allow you to learn Charms Spell. These spells are usually very general and can range from wide variety of usage, like tools, simple defense and even powerful spells.",
    "skillpointsCost": 40
}
```
### Response Body
```json
{
    "classId": 1,
    "className": "Charms",
    "classDescription": "This class room allow you to learn Charms Spell. These spells are usually very general and can range from wide variety of usage, like tools, simple defense and even powerful spells.",
    "skillpointsCost": 40
}
```
Status Code: 201 Created
### Error Handling:
If the request body is missing className, classDescription and skillpointsCost, return 400 Bad Request.

If the provided class name is already associated with another class name, return 409 Conflict.

## 2: GET /class
Retrieve a list of all classes
### Response Body
```json
[
    {
        "class_id": 1,
        "className": "Charms",
        "classDescription": "This class room allow you to learn Charms Spell. These spells are usually very general and can range from wide variety of usage, like tools, simple defense and even powerful spells.",
        "randomizedSpell_id": null,
        "skillpointsCost": 40,
        "spellbooks_id": null
    },
    {
        "class_id": 2,
        "className": "Dark Arts",
        "classDescription": "This class room allow you to learn Dark Arts. ",
        "randomizedSpell_id": null,
        "skillpointsCost": 40,
        "spellbooks_id": null
    },
    {
        "class_id": 3,
        "className": "Martial Arts",
        "classDescription": "This class room allow you to learn Martial Arts. ",
        "randomizedSpell_id": null,
        "skillpointsCost": 40,
        "spellbooks_id": null
    },
    {
        "class_id": 4,
        "className": "Transfiguration",
        "classDescription": "This class room allow you to learn Transfiguration. ",
        "randomizedSpell_id": null,
        "skillpointsCost": 70,
        "spellbooks_id": null
    },
    {
        "class_id": 5,
        "className": "Psychic",
        "classDescription": "This class room allow you to learn Psychic. ",
        "randomizedSpell_id": null,
        "skillpointsCost": 60,
        "spellbooks_id": null
    },
    {
        "class_id": 6,
        "className": "Elemental",
        "classDescription": "This class room allow you to learn Elemental. ",
        "randomizedSpell_id": null,
        "skillpointsCost": 60,
        "spellbooks_id": null
    },
    {
        "class_id": 7,
        "className": "Cursed Technique",
        "classDescription": "This class room allow you to learn Cursed Technique. ",
        "randomizedSpell_id": null,
        "skillpointsCost": 70,
        "spellbooks_id": null
    }
]
```
Status Code: 200 OK

## 3: GET /class/{type1}/type/filter
Retrieve a list of spells in that class based on their type, showing their cost, spell_id, spellname, type and spellInfo.

For example, I want to filter the spell by Psychic type, then adjust the params accordingly.
### Response Body
```json
[
    {
        "cost": 60,
        "spell_id": 14,
        "spellname": "Psychic Limbs",
        "type": "Psychic",
        "spellInfo": "The first step to harnessing your own psychich power by creating long tangible arms as tool or defense"
    },
    {
        "cost": 60,
        "spell_id": 15,
        "spellname": "Lunar Synthesis",
        "type": "Psychic",
        "spellInfo": "User is able to heal wounds by embracing the moonlight."
    }
]
```
Status Code: 200 OK

### Error Handling:
If the requested type does not exist, return 404 Not Found.

## 4: GET /class/{className}/className/{type1}/random
Retrieve a random spell to check through based on className and type1. 

Backstory: I originally wanted to make a Gacha type system so the person can get buy a random spell. But it did not work. So i repurpose it to another controller.
### Response Body
```json
{
    "message": "Random spell selected",
    "spell": {
        "class_id": 6,
        "className": "Elemental",
        "classDescription": "This class room allow you to learn Elemental. ",
        "cost": 60,
        "spell_id": 16,
        "spellname": "Blossoming Love",
        "type": "Elemental",
        "spellInfo": "A gentle spell that summons radiant flowers to bloom around the target, soothing their pain and healing their wounds with a warm, comforting energy."
    }
}
```
Status Code: 200 OK
### Error Handling: 
If Class and type are mismatched, return 403 Forbidden.

## 5: POST /class/{type1}/{className}/purchase/{spellbooks_id}/spellbooks
Create a request with the following data in the request body, randomizedSpell_id, which is the spell id you want to buy. The spell must belong to the Class and type to work. If uncertain, user can check the spell record filters.
### Example Request Body
```json
{
    "randomizedSpell_id": 5
}
```
### Response Body
```json
{
    "message": "Spell purchased successfully!",
    "data": {
        "className": "Dark Arts",
        "type1": "Dark Arts",
        "spellbooks_id": 2,
        "purchasedSpell_id": 5
    }
}
```
Note: randomizedSpell_id is the same as purchasedSpell_id.

Status Code: 201 Created
### Error Handling:
If the request body is missing randomizedSpell_id, return 400 Bad Request.

If Class, type and randomizedSpell_id are mismatched, return 403 Forbidden.

# Player 
## 1: POST /player/createPlayer/{user_id}
Create a request with player_name and the user id of who that player belongs to in url.
### Example Request Body
```json
{
    "player_name": "Player One"
}
```
### Response Body
```json
{
    "user_id": 1,
    "player_name": "Player One"
}
```
Status Code: 201 Created
### Error Handling:
If the request body is missing player_name, return 400 Bad Request.

## 2: PUT /player/{player_name}/{spellbooks_id}/spellbooksLink
Update spells details by providing `player_name` and  `spellbook_id` in the URL. (First method for linking spellbook to player)

Note: This is because when we post the player, we did not post the spellbook id to use first. Hence, PUT method can allow us to update the player by putting the spellbook we want the player to use. Note that player can have more than one spellbook, allowing them to edit and change the spellbook they want.

### Example Request Url
```json
http://localhost:3002/player/Player One/2/spellbooksLink
```
Meaning: I want Player One to use spellbook with an ID of 2 for battle.

### Response Body
```json
{
    "message": "Spellbook successfully linked to player by player name.",
    "player_name": "Player One",
    "spellbooks_id": 2
}
```
Status Code: 200 OK
### Error Handling:
If the requested Player does not exist, return 404 Not Found.

## 3: PUT /player/{player_id}/{spellbooks_id}/playerIDLink
Update spells details by providing `player_id` and  `spellbook_id` in the URL. (Second method for linking spellbook to player)
### Example Request Url
```json
http://localhost:3002/player/1/4/playerIDLink
```
Meaning: I want player_id 1 which is Player One to use spellbook with an ID of 4 for battle.
### Response Body
```json
{
    "message": "Spellbooks successfully linked to player by player id.",
    "player_id": 1,
    "spellbooks_id": 4
}
```
Status Code: 200 OK
### Error Handling:
If the requested Player does not exist, return 404 Not Found.

## 4: GET /player/spellDeckPlayer/{player_id}
Retrieve a player based on their player id, showing their spells inside their spellbook.
### Example Url
```json
http://localhost:3002/player/spellDeckPlayer/1
```
Meaning: I want to see what spells does the player use.
### Response Body
```json
{
    "message": "Spellbook Info retrieved successfully!",
    "data": [
        {
            "spell_id": 5,
            "name": "Umbra Tenebris",
            "type": "Dark Arts",
            "ability": "Wrap the victim's heart with dark tendrils, locking and tightening their heart from pumping blood if they even move a single inch.",
            "damage": 20,
            "heal": 0,
            "effect": "poison"
        },
        {
            "spell_id": 6,
            "name": "Shou Ling Tong",
            "type": "Dark Arts",
            "ability": "A punishing spell created to targets the nerves in the victim's hand, sending waves of excruciating pain every time they attempt to touch anything or casting a spell.",
            "damage": 30,
            "heal": 0,
            "effect": "poison"
        },
        {
            "spell_id": 7,
            "name": "Sanguinem Blood",
            "type": "Dark Arts",
            "ability": "User is able to manuplate it's own blood into various forms as weapons or armor, bombs and increasing blood flow..",
            "damage": 30,
            "heal": 30,
            "effect": null
        },
        {
            "spell_id": 1,
            "name": "Iuvenaleaqua",
            "type": "Charms",
            "ability": "A simple cast of fresh water that provide a soothing healing relieve to injuries.",
            "damage": 0,
            "heal": 20,
            "effect": null
        },
        {
            "spell_id": 17,
            "name": "Thousand Petal Dance",
            "type": "Elemental",
            "ability": "Summons a storm of razor-sharp petals that swirl gracefully around the caster, cutting enemies in range.",
            "damage": 60,
            "heal": 60,
            "effect": null
        },
        {
            "spell_id": 16,
            "name": "Blossoming Love",
            "type": "Elemental",
            "ability": "A gentle spell that summons radiant flowers to bloom around the target, soothing their pain and healing their wounds with a warm, comforting energy.",
            "damage": 0,
            "heal": 80,
            "effect": null
        }
    ]
}
```
Status Code: 200 OK
### Error Handling:
If the requested player_id does not exist, return 404 Not Found.

## 5: GET /player/searchPlayer/{user_id}
Retrieve a player based on their player id, showing their player_id, player_name, spellbooks_id, owner_id, username.

### Example Url
```json
http://localhost:3002/player/searchPlayer/1
```
Meaning: I want to search for a player information that have player id of 1.

Note: spellbooks_id is the spellbook that player will use. owner id is the user id that made that player, username is the username of the user. 
### Response Body
```json
[
    {
        "player_id": 1,
        "player_name": "Player One",
        "spellbooks_id": 2,
        "owner_id": 1,
        "username": "socuser321"
    }
]
```
Status Code: 200 OK
### Error Handling
If the requested player_id does not exist, return 404 Not Found.

# Enemy 
## 1: POST /enemy
Create a request with enemy_name, enemy_health, default_health, enemy_info, skillpoints_reward and difficulty.
### Example Request Body (Enemy that can use all spells from Spell table)
```json
{
    "enemy_id": 1,
    "enemy_name": "Muggle",
    "enemy_health": 20,
    "enemy_info": "The average powerless human with no experience on using magic. Please don't destory him",
    "skillpoints_reward": 10,
    "difficulty": "easy",
    "default_health": 20
}
```

We can customised our enemy stats even more by adding optional data such as damage_max, damage_min, heal_max, heal_min and specialist

## Example 1: Enemy with damage range and specialist filter

```json
{
    "enemy_id": 1,
    "enemy_name": "Magie Vellarim",
    "enemy_health": 100,
    "enemy_info": "A female witch fallen to the tempatation of abusing dark arts and cursed spells to do crimes.",
    "skillpoints_reward": 100,
    "difficulty": "hard",
    "default_health": 100,
    "damage_max": 100,
    "damage_min": 20
}
```

## Example 2: Enemy with heal range.
```json
{
    "enemy_id": 2,
    "enemy_name": "Bignose Pharacist",
    "enemy_health": 150,
    "enemy_info": "A bignosed villager that supplies the local village with herbs and medicine. Expect her to be stocked with health and potions",
    "skillpoints_reward": 70,
    "difficulty": "hard",
    "default_health": 150,
    "heal_max": 100,
    "heal_min": 100
}
```

## Example 3: Enemy with damage and heal range, with specialist filter.
```json
{
    "enemy_id": 3,
    "enemy_name": "Alakadarva",
    "enemy_health": 100,
    "enemy_info": "A psychic user that isolated itself in caves, practicing all forms of psychic magic. Expect your brain to turn to mush.",
    "skillpoints_reward": 100,
    "difficulty": "medium",
    "default_health": 100,
    "damage_max": 100,
    "damage_min": 20,
    "heal_max": 100,
    "heal_min": 100
}
```

Status Code: 200 OK

### Error Handling:
If the request body have the same enemy name, return 409 Conflict.

If the request body have missing fields, return 400 Bad Request

If the request body have incorrect range value, return 400 Bad Request


## 2: PUT /enemy/{enemy_id}
Update enemy details by providing their details and optional stats for customization.
### Example URL
```json
http://localhost:3002/enemy/4
```

### Example Request Body
```json
{
    "enemy_id": 4,
    "enemy_name": "Goblin Shamans",
    "enemy_health": 200,
    "default_health": 200,
    "enemy_info": "The local village has contacted you on nearby goblins harassing villagers, destorying crops, stealing and even raiding.",
    "skillpoints_reward": 120,
    "difficulty": "hard",
    "damage_max": 60,
    "damage_min": 30
}
```

### Response Body
```json
{
    "enemy_id": 4,
    "enemy_name": "Goblin Shamans",
    "enemy_health": 200,
    "default_health": 200,
    "enemy_info": "The local village has contacted you on nearby goblins harassing villagers, destorying crops, stealing and even raiding.",
    "skillpoints_reward": 120,
    "difficulty": "hard",
    "damage_max": 60,
    "damage_min": 30
}
```

Status Code: 200 OK

### Error Handling:
If the request body have the same enemy name, return 409 Conflict.

If the request body have missing fields, return 400 Bad Request

If the request body have incorrect range value, return 400 Bad Request

If the requested player_id does not exist, return 404 Not Found.

## 3: GET /enemy/{enemy_id}
Retrieve an enemy's data based on their enemy id, showing their enemy_id, enemy_name, enemy_health, default_health, enemy_info, skillpoints_reward, difficulty and more.

### Response Body
```json
[
    {
        "enemy_id": 19,
        "enemy_name": "The Devil",
        "enemy_health": 100,
        "default_health": 100,
        "enemy_info": "Evil guy",
        "skillpoints_reward": 200,
        "difficulty": "medium",
        "damage_min": 10,
        "damage_max": 100,
        "heal_min": 10,
        "heal_max": 100,
        "specialist": null
    }
]
```
Status Code: 200 OK
### Error Handling:
If the requested enemy_id does not exist, return 404 Not Found.

# CombatRef 
## How the controllers come together and steps to work:
1: User first decide which player battle which enemy by their ID

2: Player and Enemy take turns to attack or heal. One action per turn.

3: Player start first. Attack or Healing

4: Enemy continue. Attack or Healing

5: Within that, Player can check health status.

6: Repeat Step 3 and 4 or 5 

7: If Player win, get skillpoints reward

8: Reset both side health.

9: Repeat

## 1: POST /player/{player_id}/enemy/{enemy_id}
Create a battle versus date with the following data in the URL, player_id and enemy_id.

The player_id is the one that the user choose to initate the battle, the enemy_id is the one that user want to fight against.

### Example URL
```json
http://localhost:3002/combat/player/1/enemy/1
```

This means player 1 wants to fight enemy 1. This is needed to start the battle or else the battle will not work.

### Response Body
```json
{
    "message": "Battle started successfully!",
    "player_id": 1,
    "enemy_id": 1
}
```
Status Code: 200 OK

### Error Handling:
If the requested player_id does not exist, return 404 Not Found.

If the requested enemy_id does not exist, return 404 Not Found.

## 2: PUT /player/{player_id}/enemy/{enemy_id}/attackEnemy
Update enemy details by providing their enemy and player id to show Player attacking Enemy using spells inflicting damage to Enemy
### Url Example:
```json
http://localhost:3002/combat/player/1/enemy/1/attackEnemy
```
This means player 1 wants to attack enemy 1, and the attacking spell is randomly selected and applied.

The spell is filter through the Spell Table, with accordance to the spells record inside that Spellbook Id that is linked with player 1 by using a Junction Table, with optional range such as damage range and specialist.

### Response Body
```json
{
    "message": "Spell has been selected and applied.",
    "player_id": 1,
    "enemy_id": 1,
    "spell": [
        {
            "spell_id": 6,
            "spell_name": "Shou Ling Tong",
            "spell_info": "A punishing spell created to targets the nerves in the victim's hand, sending waves of excruciating pain every time they attempt to touch anything or casting a spell.",
            "damage": 30
        }
    ]
}
```
Status Code: 200 OK

### Error Handling:
If the requested player_id does not exist, return 404 Not Found.

If the requested enemy_id does not exist, return 404 Not Found.

If requested player_id or enemy_id health drop to 0, return 428 Precondition Required to stop battle.

## 3: PUT /player/{player_id}/healPlayer
Update player details by providing their player id to show Player is being heal.
### Example URL
```json
http://localhost:3002/combat/player/1/healPlaye
```
This means player 1 wants to heal based on the Healing spells recorded on his spellbooks ID by using a Junction Table. A random healing spell is selected and applied to Player.

### Response Body
```json
{
    "message": "Healing spell selected and applied.",
    "player_id": 1,
    "spell": {
        "spell_id": 16,
        "spell_name": "Blossoming Love",
        "spell_info": "A gentle spell that summons radiant flowers to bloom around the target, soothing their pain and healing their wounds with a warm, comforting energy.",
        "heal": 80
    }
}
```
Status Code: 200 OK

### Error Handling:
If the requested player_id does not exist, return 404 Not Found.

If requested player_id health is already 0, return 428 Precondition Required to stop battle because it is cheating to heal when you are defeated.

## 4: PUT /enemy/{enemy_id}/player/{player_id}
Update player details by providing their enemy and player id to show Enemy attacking Player using spells inflicting damage to Player
### Url Example
```json
http://localhost:3002/combat/enemy/1/player/1
```
### Response Body
```json
{
    "message": "Spell has been selected and applied.",
    "player_id": 1,
    "enemy_id": 1,
    "spell": [
        {
            "spell_id": 5,
            "spell_name": "Umbra Tenebris",
            "spell_info": "Wrap the victim's heart with dark tendrils, locking and tightening their heart from pumping blood if they even move a single inch.",
            "damage": 20
        }
    ]
}
```
Status Code: 200 OK
If the requested player_id does not exist, return 404 Not Found.

If the requested enemy_id does not exist, return 404 Not Found.

If requested player_id or enemy_id health drop to 0, return 428 Precondition Required to stop battle. 

## 5: PUT /enemy/{enemy_id}/healEnemy
Update enemy details by providing their enemy id to show Enemy is being heal.
### Url Example
```json
http://localhost:3002/combat/enemy/1/healEnemy
```
### Response Body
```json
{
    "message": "Healing spell selected and applied.",
    "enemy_id": 1,
    "spell": {
        "spell_id": 8,
        "spell_name": "Avada Exterminus",
        "spell_info": "One of the banned spells in the wizarding community that can get you jailed. It forcefully rip the soul out from the victim' body so do the caster in a metaphorically way.",
        "heal": 50
    }
}
```
Status Code: 200 OK
If the requested enemy_id does not exist, return 404 Not Found.

If requested enemy_id health drop to 0, return 428 Precondition Required to stop battle. 

## 6: PUT /restoreHealth/player/{player_id}/enemy/{enemy_id}
Update player and enemy details by providing their player and enemy id to restore their health to default health. (Max health). 

This allows both side to continue fighting when one of them are defeated, or reset battle.
### URL Example
```json
http://localhost:3002/combat/restoreHealth/player/1/enemy/1
```
Because Player 1 and Enemy 1 has fought and lose some health, they can restore to fight again or reset.

Player can also reset if they want to fight a new Enemy by providing a new Enemy id in the startBattle controller.

### Response Body
```json
{
    "message": "Health restored successfully for both sides."
}
```
Status Code: 200 OK

### Error Handling:
If the requested player_id does not exist, return 404 Not Found.

If the requested enemy_id does not exist, return 404 Not Found.

## 7: PUT /putRewards/player/{player_id}/enemy/{enemy_id}
Update User skillpoints if Player id connected to User id won the battle against Enemy when Enemy health drop to 0.
### Url Example
```json
http://localhost:3002/combat/getRewards/player/1/enemy/1
```
Player 1 wants to get skillpoints reward after enemy 1 is defeated. The controller and model checks for enemy health = Null or 0, and add the skillpoints value to User. 

### Response Body
```json
{
    "message": "Skillpoints successfully added to player. Congrates!"
}
```

Status Code: 200 OK
### Error Handling:
If the requested player_id does not exist, return 404 Not Found.

If the requested enemy_id does not exist, return 404 Not Found.

If requested enemy_id health is not NULL or 0, return 428 Precondition Required to stop user from getting skillpoints reward. 

## 8: GET /player/{player_id}/enemy/{enemy_id}/health
Retrieve a player and enemy based on their id, showing their their id and health to check battle status and who is winning and future decision making.

### Url Example
```json
http://localhost:3002/combat/player/1/enemy/1/health
```
### Response Body
```json
{
    "message": "Health Stats:",
    "data": [
        {
            "player_id": 1,
            "player_health": 100,
            "enemy_id": 1,
            "enemy_health": 100
        }
    ]
}
```
Status Code: 200 OK
### Error Handling:
If the requested player_id does not exist, return 404 Not Found.

If the requested enemy_id does not exist, return 404 Not Found.

# Leaderboard 
## 1: GET /leaderboard/rankUser
Retrieve the top 3 users with the most skillpoints. The leaderboard is sorted in descending order.
### Response Body
```json
{
    "message": "Top 3 Users with most skillpoints",
    "data": [
        {
            "username": "guan ying",
            "skillpoints": 200
        },
        {
            "username": "Danny",
            "skillpoints": 120
        },
        {
            "username": "socuser321",
            "skillpoints": 0
        }
    ]
}
```
Status Code: 200 OK

## 2: GET/leaderboard/rankSpell
Retrieve the top 3 spells with the most skillpoints. The leaderboard is sorted in descending order.
### Response Body
```json
{
    "message": "Top 3 Users with most skillpoints",
    "data": [
        {
            "ownerUsername": "socuser321",
            "spellbooks_name": "FIRST SPELLBOOKS",
            "spells_count": 2
        },
        {
            "ownerUsername": "guan ying",
            "spellbooks_name": "SECOND SPELLBOOKS",
            "spells_count": 1
        }
    ]
}
```
Status Code: 200 OK