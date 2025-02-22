<div align="center">
  <h1>League of Legends Match Outcome Prediction</h1>
  <img src="images/lol_logo.png" alt="LoL Logo" width="600"/>
</div>

# Introduction

✨ League of Legends is one of my favorite video games, and I've been interested in understanding how much the first few minutes of the game impact its outcome. So I decided to start this project in my spare time.

This project employs a predictive model to forecast the outcome (victory or defeat) of a League of Legends match (Blue Team Vs Red Team) using data gathered from the first 10 minutes of gameplay. The model is deployed using a Flask server, allowing you to select your preferred input parameters.

<div align="center">
  <img src="images/interface.png" alt="Interface" width="600"/>
</div>

# Information
_(If you already know the game, please just go to the Installation section below!)_

If you're unfamiliar with the game League of Legends or various key parameters of a match, here are explanations on how the game works and the meaning of the features used as inputs for the model.

League of Legends is a Multiplayer Online Battle Arena (MOBA) where 2 teams of 5 players **(Blue team vs Red team)** compete to destroy the opposing team's base. Each player controls 1 champion with unique abilities, aiming to accumulate resources (Gold, Dragons, Towers, ...) to become stronger and defeat the opposing team. It is one of the games known for its highly complex tactical aspects.

- **Gold 🪙:** In-game currency earned by players to buy items that enhance their champion's abilities.
- **FirstBlood 🩸:** The first kill in the game, which grants bonus gold to the player or team that achieves it.
- **Kills ❌:** Number of enemy champions a player has defeated (each kill gives gold).
- **Deaths 💀:** Number of times a player's champion has been defeated by an enemy.
- **Assists ✅:** Number of times a player has contributed to defeating an enemy champion without landing the killing blow (each assist gives gold).
- **Dragons 🐉:** Powerful neutral monsters on the map that grant team-wide buffs when killed (each Dragon also gives gold/exp to all players).
- **Experience 🆙:** Points accumulated by a champion to level up and improve their abilities throughout the game (each level makes your champion stronger)
- **Towers 🗿:** Defensive structures located along the lanes that players must destroy to advance toward the enemy's base (each tower destroyed gives gold)

# Comments

The accuracy of our model is around 73%, which may seem low at first glance. However, a game of League of Legends lasts on average 20/25 minutes and thanks to my game knowledge, I know that the individual performances of the players (especially their decision-making and their skills) have a significant impact on the game and can change its outcome despite a purely theoretical deficit.

Therefore, an accuracy of 73% actually makes sense in the context of this game as so much can happen in the next 10/15 minutes.

# Installation

Use a dedicated environnement to install the librairies.

Clone repo :
```
git clone https://github.com/MaxLSB/LoL-Game-Win-Prediction.git
```

Install the requirements for the app:
```
pip install -r requirements.txt
```

Scripts must be executed from the root folder of the project, be careful about the paths!

Launching the server:
```
python app.py
```

Connect to the server:
```
http://127.0.0.1:5000/
```
<h2> Change the values of the features as you please and predict the game outcome! </h2>
