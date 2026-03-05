
# ChantsAdventure

**ChantsAdventure** is a text-based adventure game written in C++. Embark on a thrilling journey through a mysterious world filled with monsters, treasures, and hidden secrets. Navigate through various locations, collect assets, battle monsters, and strive to reach the Hidden Temple to win the game.


## Features

- **Exploration**: Traverse through a map of interconnected locations, each with unique descriptions.
- **Assets**: Collect various assets scattered across locations to aid in your adventure.
- **Monsters**: Encounter and battle different monsters with varying strengths.
- **Combat System**: Engage in combat using a simple fight mechanism based on fight coefficients.
- **Inventory Management**: Pick up and drop assets as needed.
- **Win Condition**: Collect specific assets and reach the Hidden Temple to win the game.

## Project Structure

```
ChantsAdventure/
├── app/
│   ├── CMakeLists.txt
│   └── game.cpp
├── inc/
│   ├── AdventureGameMap.hpp
│   ├── Asset.hpp
│   ├── Combatant.hpp
│   ├── Monster.hpp
│   ├── Node.hpp
│   └── Player.hpp
├── src/
│   ├── AdventureGameMap.cpp
│   ├── Asset.cpp
│   ├── Combatant.cpp
│   ├── Monster.cpp
│   ├── Node.cpp
│   └── Player.cpp
├── tests/
│   ├── CMakeLists.txt
│   └── adventuretests.cpp
├── CMakeLists.txt
├── LICENSE
└── README.md
```

- **app/**: Contains the main application code (game.cpp) and its CMake configuration.
- **inc/**: Header files for classes used in the game.
- **src/**: Source files implementing the game logic.
- **tests/**: Unit tests for the project using Google Test framework.
- **CMakeLists.txt**: Top-level CMake configuration file.
- **LICENSE**: The project's license.
- **README.md**: Project documentation.

## Dependencies

- **C++ Compiler**: Compatible with C++14 standard (e.g., GCC, Clang, MSVC).
- **CMake**: Version 3.10 or higher.
- **Google Test**: For running unit tests.  
  _Note_: Instructions are provided to include Google Test as part of the build process.



## Running the Game

After building the project, you can run the game using the following command:

```bash
./app/ChantsAdventure
```

## Gameplay Instructions

- **Objective**: Collect the "Hammer" and "Purple Haze" assets and reach the "Hidden Temple" to win the game.
- **Commands**:
  - **Movement**: Enter the node ID to move to a connected location.
  - **Take Asset**: `t <asset_name>` (e.g., `t hammer`) to pick up an asset at the current location.
  - **Drop Asset**: `d <asset_name>` to drop an asset from your inventory at the current location.
  - **Attack Monster**: `a <monster_name>` to attack a monster present at the current location.
  - **Inspect Asset**: `i <asset_name>` to read the description of an asset in your inventory or at the current location.
  - **Exit Game**: `x` to exit the game.

- **Tips**:
  - **Health Management**: Keep an eye on your health. If it drops to zero, the game is over.
  - **Assets**: Some assets are offensive and can help you in battles.
  - **Exploration**: Explore different locations to find assets and avoid or confront monsters.

## Testing

The project includes unit tests using the Google Test framework.



## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Enjoy your adventure! If you encounter any issues or have suggestions for improvements, feel free to open an issue or contribute to the project.
