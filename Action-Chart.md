# Action Charts for Serpent Clash

## 1. Game Start

| Action                | Trigger                     | Outcome                                    |
|-----------------------|-----------------------------|--------------------------------------------|
| Player opens the game | Game Launch                  | Display Welcome Screen                     |
| Player clicks "Start" | Start button clicked         | Load Game and initialize user data         |
| Player clicks "Shop"  | Shop button clicked          | Open Shop menu                             |
| Player clicks "Settings" | Settings button clicked      | Open Settings menu                         |
| Player clicks "Credits" | Credits button clicked       | Show Credits screen                        |
| Player clicks "Exit"   | Exit button clicked          | Close the game application                 |

## 2. Welcome Screen Actions

| Action                | Trigger                     | Outcome                                    |
|-----------------------|-----------------------------|--------------------------------------------|
| Player selects "Start" | Start button clicked         | Begin game preparation                    |
| Player selects "Shop"  | Shop button clicked          | Open Shop for upgrades and boosts          |
| Player adjusts "Settings" | Settings changed             | Apply settings changes (music, controls)   |
| Player views "Credits" | Credits viewed               | Display credits                            |
| Player exits           | Exit button clicked          | Close the game                             |

## 3. In-Game Actions

| Action                | Trigger                     | Outcome                                    |
|-----------------------|-----------------------------|--------------------------------------------|
| Player moves the snake | Player input (keyboard/mouse) | Update snake position                     |
| Player collects power-ups | Power-up collected           | Apply power-up effects                     |
| Player encounters boss | Boss appears                 | Initiate Boss Fight                        |
| Player defeats mini-boss | Mini-boss defeated           | Award coins                                |
| Player defeats the boss | Boss defeated                | Award coins, advance to next level         |
| Player's snake dies    | Snake collision              | End game session, show game over screen    |

## 4. Boss Fight Mechanics

| Action                | Trigger                     | Outcome                                    |
|-----------------------|-----------------------------|--------------------------------------------|
| Boss appears          | Boss encounter               | Boss spawns with power-ups and power-downs |
| Boss uses power-ups   | Boss action                  | Boss applies power-up effects              |
| Player uses power-ups | Player action                | Player applies power-up effects            |
| Player uses special abilities | Special ability used        | Player deals damage or gains advantage    |
| Boss uses power-downs | Boss action                  | Boss applies power-down effects            |
| 2 minutes survival time | Timer starts                 | Survival mode for 2 minutes                |
| 30 seconds preparation time | Timer ends                   | Enhanced power-ups and food available      |

## 5. Bonus Level Actions

| Action                | Trigger                     | Outcome                                    |
|-----------------------|-----------------------------|--------------------------------------------|
| Player enters bonus level | Level completed              | Start 15-second coin collection game      |
| Player collects coins  | Coin collected               | Increase coin count                       |
| Time ends              | 15 seconds elapsed          | End bonus level, return to game            |
| Coins used             | Purchase in shop             | Unlock boosts and customizations           |

## 6. Shop Interactions

| Action                | Trigger                     | Outcome                                    |
|-----------------------|-----------------------------|--------------------------------------------|
| Player opens Shop      | Shop button clicked          | Display available boosts and upgrades      |
| Player purchases item  | Purchase button clicked      | Deduct coins, apply upgrade/boost          |
| Player customizes snake | Customization selected       | Apply snake customization                  |

## 7. Game Over Actions

| Action                | Trigger                     | Outcome                                    |
|-----------------------|-----------------------------|--------------------------------------------|
| Snake dies            | Collision/Time up            | Display Game Over screen                  |
| Player restarts game  | Restart button clicked       | Reset game state and start new session    |

---

For more information, refer to the [Game Configuration](Game-Configuration.md) and [Game Models](Game-Models.md).
