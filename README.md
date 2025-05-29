# SetCardGame

A Java implementation of the Set card game with a graphical user interface, supporting both human and machine based players. The game features multithreaded logic, configurable settings, and real-time interaction.
The game's rules can be found here: https://en.wikipedia.org/wiki/Set_(card_game)

## Getting Started

1. **Make sure Java is installed** (version 1.8 or later).
2. **Clone or download** the repository to your local machine.
3. **Edit the configuration file** at `/src/main/resources/config.properties` as needed:
    - `HumanPlayers`: Number of human players.
    - `ComputerPlayers`: Number of computer players.
    - `Hints`: `True`/`False` — show legal sets currently visible on the table.
    - `PlayerNames`: Players' names, separated by `, ` (see example in file).
    - `TurnTimeoutSeconds`:
        - `> 0`: Regular countdown timer mode (default is 60 seconds).
        - `= 0`: "Free play" mode (no timer).
        - `< 0`: "Elapsed" mode (timer resets after a legal set is collected).

## Commands

- **To compile:**  
  ```
  mvn clean compile test
  ```

- **To run:**  
  ```
  java -cp target/classes bguspl.set.Main
  ```

## How to Play

- Human players interact via keyboard:
 ![image](https://github.com/user-attachments/assets/f48d20c9-efa1-41c9-add9-df9a05f98f43)
- Machine based players act automatically.
- The User Interface:
  ![image](https://github.com/user-attachments/assets/ccb58012-2dce-400f-884a-033bdaa1f347)
- Place tokens to select cards and try to find valid sets.
- The game manages scoring, penalties, and turn logic automatically.




