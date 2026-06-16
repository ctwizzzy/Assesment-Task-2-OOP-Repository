# Software Engineering Assessment Task 2



## <b> Part A </b>

## Attributes chosen

- Price

  I chose price as it is one of the most importanrt attributes to the game. Each card has a certain price and players are given a budget to spend on cards. The better the car is, the higher it's price will be so players should pick wisely when to save or spend money.
- Acceleration (0 to 100 km/h)

  Acceleration is an attribute that the card will have. It measures how quickly a car can go from from 0 to 100 km/h. Acceleration is the second most important attribute in the game and gives 40 points if won. I chose acceleration as it is a playable attribute about performance of the car and is important to gameplay. 
- Top Speed

  Top speed is another attribute the card will have. It measures the absolute top speed the car can go (km/h). Top speed is the most important attribute in the game and gives 50 points if won. I chose top speed as it is the most important attribute in the game as it tells us the absolute fastest speed the car can go and is a playable attribute, making it important to gameplay.
- Model
  
  Model shows what model from the specific brand the car is. For example, the brand is Lamborginhi and the model is Aventador. Model is not a playable attribute with which players will battle, but simly an attribute to describe the car. I chose model as it is an important description of the car as it tells us the specific model the car is. 
- Make
  
  Make is the brand of the car that built the vehicle. For example, Toyota, Subaru, Lamborginhi etc. Like model, make is not a playable attribute and is simply a description of the car. I chose make as an attribute as it tells us what brand the car is from, a very important detail when describing cars. 

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
| safety_features() | Method for the car to have safety features

Role of car: Car is the data that is on the cards. Car holds 6 attributes amd 2 methods. 

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




