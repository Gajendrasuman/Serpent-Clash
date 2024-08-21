# Game Models for Serpent Clash

## 1. User Model

**Collection Name:** `users`

| Field            | Type      | Description                                       |
|------------------|-----------|---------------------------------------------------|
| `username`       | String    | Unique identifier for the user.                  |
| `passwordHash`   | String    | Hashed password for authentication.               |
| `coins`          | Number    | Total coins the user has.                        |
| `levelsUnlocked` | Array of Numbers | List of levels unlocked by the user.         |
| `settings`       | Object    | User's settings for the game.                     |
| `createdAt`      | Date      | Timestamp when the user was created.             |

## 2. Game State Model

**Collection Name:** `gameStates`

| Field            | Type      | Description                                       |
|------------------|-----------|---------------------------------------------------|
| `userId`         | ObjectId  | Reference to the `users` collection.             |
| `level`          | Number    | Current level of the game.                       |
| `snakeState`     | Object    | Current state of the snake.                      |
| `bossState`      | Object    | Current state of the boss.                       |
| `powerUps`       | Array of Strings | List of active power-ups.                   |
| `startTime`      | Date      | Timestamp when the game started.                 |
| `endTime`        | Date      | Timestamp when the game ended.                   |

## 3. Boss Model

**Collection Name:** `bosses`

| Field            | Type      | Description                                       |
|------------------|-----------|---------------------------------------------------|
| `level`          | Number    | Level at which the boss appears.                 |
| `health`         | Number    | Boss's health points.                            |
| `powerUp`        | String    | Power-up the boss has (e.g., `speedBoost`).      |
| `powerDown`      | String    | Power-down the boss has (e.g., `slowDown`).      |
| `specialAbilities` | Array of Strings | Special abilities of the boss (e.g., `fireBreath`). |
| `appearance`     | String    | Description or reference for the boss's appearance.|

## 4. Power-Up Model

**Collection Name:** `powerUps`

| Field            | Type      | Description                                       |
|------------------|-----------|---------------------------------------------------|
| `type`           | String    | Type of power-up (e.g., `speedBoost`, `shield`). |
| `duration`       | Number    | Duration of the power-up in seconds.             |
| `effect`         | String    | Effect of the power-up (e.g., `increaseSpeed`).  |
| `permanent`      | Boolean   | Whether the power-up is permanent or temporary.  |

## 5. Coin Transaction Model

**Collection Name:** `coinTransactions`

| Field            | Type      | Description                                       |
|------------------|-----------|---------------------------------------------------|
| `userId`         | ObjectId  | Reference to the `users` collection.             |
| `amount`         | Number    | Number of coins involved in the transaction.     |
| `transactionType`| String    | Type of transaction (e.g., `bossDefeat`, `bonusLevel`). |
| `transactionDate`| Date      | Timestamp of the transaction.                    |

---

For more details, refer to the [Game Configuration](Game-Configuration.md) and [Action Charts](Action-Chart.md).
