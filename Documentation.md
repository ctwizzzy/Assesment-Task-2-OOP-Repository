# Software Engineering Assessment Task 2



## <b> Part A </b>

## Attributes chosen

- Price

  I chose price as it is a good description of the cards and their value. Price is simply a description and not a playable attribute. Price is the 6th most important attribute. 
- Acceleration (0 to 100 km/h)

  Acceleration is an attribute that the card will have. It measures how quickly a car can go from from 0 to 100 km/h. Acceleration is the 2nd most important attribute in the game. I chose acceleration as it is a playable attribute about performance of the car and is important to gameplay. 
- Top Speed

  Top speed is another attribute the card will have. It measures the absolute top speed the car can go (km/h). Top speed is the most important attribute in the game and gives 50 points if won. I chose top speed as it is the most important attribute in the game as it tells us the absolute fastest speed the car can go and is a playable attribute, making it important to gameplay.
- Model
  
  Model shows what model from the specific brand the car is. For example, the brand is Lamborginhi and the model is Aventador. Model is not a playable attribute with which players will battle, but simly an attribute to describe the car. I chose model as it is an important description of the car as it tells us the specific model the car is. Model is the 4th most important attribute. 
- Make
  
  Make is the brand of the car that built the vehicle. For example, Toyota, Subaru, Lamborginhi etc. Like model, make is not a playable attribute and is simply a description of the car. I chose make as an attribute as it tells us what brand the car is from, a very important detail when describing cars. Make is the 5th most important attribute. 

- Power 

  Power is the amount of work the engine is capable of doing per second. Power is a playable atrribute and is meausred in horsepower (hp). Power is the third most important attribute. I chose power because it will be important to the game, due to it being a playable attirbute and something players can battle over.  


##  Part B 

The car has 6 main attrubutes

Attributes | Type | Attribute description|
|----------|------|----------------------|
| price    | Integer  | The price of the car in AUD
| acceleration| Integer | How fast the car can acclerate from 0 to 100 km/h
| top_speed | Integer | The absolute maximum speed the car can reach 
| model     | String  | Shows what model from the brand that made the car is 
| make      | String  | Shows what specific brand built the car
| power     | Integer | Shows the amount of work the engine is able to in a second

Methods | Description of method|
|-------|----------------------|
| drive() | The ability for the car to drive
| battle() | Battle other cars


Role of car: Car is the data that is on the cards. Car holds 6 attributes and 2 methods. 

Card: 

Attributes | Type | Attribute description |
|----------|------|-----------------------|
| car      | String | contains all the attributes of the car


Methods | Descrpition of method|
|-------|---------------------|
| hold_attributes()| Holds the data of different subclasses
| get_car() | Returns the car object back

Role of card: the role of the card is to hold the data of different subcalsses. For example, it does this with car, holding all 6 attributes and 2 methods of car. 

Deck: 

Attributes | Type | Attribute description |
|----------|------|-----------------------|
| cards    | Integer | Collection of cards within the deck

Methods | Description of method |
|-------|-----------------------|
| shuffle_deck()| Shuffle the deck randomly
| add_cards()   | Add cards to the deck
| remove_cards() | Remove cards from the deck

Role of deck:  Deck manages all the cards during the gameplay. It is able to shuffle, add and remove cards from the deck. 

Player: 

Attributes | Type | Attribute description |
|----------|------|-----------------------|
| player_name| String | Name of the player
| score| Integer| Amount of rounds won by a player


Methods | Description of method |
|-------|-----------------------|
| draw_cards()| Draw cards from the deck
| hold_cards()| Hold a certain number of cards
| select_attribute()| Select an attribute to battle on

Role of player: Player class holds data about each player and is able to draw cards, hold cards and select an attribute to battle on. 

Game: 

Attributes | Type | Attribute description |
|----------|------|-----------------------|
| deck     | Integer | Stores a deck of cards
| player_1 | String | First player
| player_2 | String | Second player
| round_number| Integer | The cuurent round number the game is on

Methods | Description of method |
|-------|-----------------------|
| start_game() | Starts the game
| play_round() | Play a round
| choose_winner() | Determine who won the round
| reset() | Finish the round and continue onto the next round
| end_game() | Finish the game

Role of game : Game is the parent class. It has the ability to start the game, play rounds, determine winners of the round, reset and move onto the next round and end the game. 


## <b> Part D </b>

This is the explanantion on how the game is to played: 

1. This is a 1v1 game. Each player is given a set of 30 cards to battle on attributes with. 


2. Both players will decide on an attribute to battle on. If they cannot agree on an attribute to battle on, they can flip a coin, heads or tails to decide which attribute to battle on. 

3. Each players will be given a choice on the card they will use to battle. At once, both players will reveal their cards and whoever has the higher or 'better' attribute wins the round and both cards are discarded from the deck.

4. In a draw, no one wins the round, and both cards are discarded from the deck. 

5. The game ends after there are no more cards remaining in the deck. Players will then count up how many rounds they won and whoever won the most rounds wins the game. 

Explanation of game balance: This keeps the game balanced as each player is given equal chances on the attribute they wish to battle on and they are allowed to choose the cards they would like to use. 

Unfair Advantage: The player who chooses the attribute to battle on could have an unfair advantage as they can select an attribute where their car is the strongest. This gives them higher control on winning the round. 

Proposed solution: Both players can alternate on the attribute they battle on each round, or can use the coin to randomly decide who chooses the attribute. This allows for both players to have higher chances of winning during each round. 

## <b> Part E </b>

The design of what the cards look like is attached in another file. 

Style Card Design: 

Top: Name of the car, model, year, price

Image section: Includes Image of the car

Mid section: Includes attributes such as acceleration, top speed and horsepower. 

Bottom Section: Includes a fun fact about the car. 

I placed name at the top as I felt top is the first thing someone reads from so it made sense to put all of those attributes such as name, model, year, price at the top. Image section is the biggest section so the image of the car should go in their. This makes sure the image is as big as possible and gives a visual representation of what the car looks like, grabbing the users attention. The midsection has all the stats and attributes as it is the main ifno that matters the most. The bottom has a func fact to add a bit more information and aesthetic about the car. 

Game UI Sketch:
Car Card comparison game|
|-----------------------|

Start Game: 

Attribute: Top speed

Card 1: 2011 Lamborghini Aventador

Card 2: 2021 Audi R8

Compare

Card 1 Top speed: 350 km/h

Card 2 Top speed: 331 km/h 

Card 1 wins!

## <b> Part F </b>

1. <u> Individual Impact </u>

    The game may influence the decision making of players when choosing cards. Players may prioritise cars with the acceleration, top speed, and horsepower as these are the attributes which win rounds. This however can affect how the user views cars in real life as this can influence them to choose cars based on performance rather than practicality and environment. As the designer, it is my responsibility to present accurate information and attributes must be based on reliable data. 

2. <u> Social Impact </u>

    This game can place social stereotypoes as it can potray super cars and the more expensive cars as more desirable. The game may also be biased towards sports cars and luxury cars than family cars, electric cars, SUVs etc due to them performing beter in terms of attributes. To make it more inclusive and fair, the game will include a wide range of cars such as sports, electric, SUV, family, luxury etc. This ensures a wide range of cars suitable to all players. The game will also be designed so that players can win mostly by strategy. 

3. <u> Environmental Impact </u> 

    Due to the game mainly rewarding high speed sports cars becuase of their attributes, players may focus on speed and power while paying less attention to environmental impacts. This could cause players in real life to favour cars with higher fuel consumption and with greater carbon emissions. The current attribute selection of the game ignores environmental impacts, focusing more on performance. To change this and encourage environmental sustainability, the game could have attributes such as electric driving range, carbon emissions and environmental impact. These attributes would reward users for being environmentally aware and encourage users to prioritise cars with a better environmental impact. 

4. <u> Legal Considerations </u>

    Many legal issues could arise from this game such as vehicle images or logos being written without permission. There are also chances that problems about information accuracy may arise. As the designer, it is my responsibility to make sure I am getting my attribute information from reliable sources. Any content which needs to be used from carsales.com.au must be used after being granted permission by them to use it. To ensure the system does not mislead users, it should display accurate information used form trusted and relaible sources. It should also be made clear that the game is for entertainment purposes only and that users must not use the information in the game as advice in vehicle purchasing. 

