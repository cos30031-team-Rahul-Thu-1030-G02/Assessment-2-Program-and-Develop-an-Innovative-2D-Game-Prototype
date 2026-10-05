# Sustainable Affairs

**Playable Build:** https://bpgg713.itch.io/sustainable-affairs

## Game Description

**Sustainable Affairs** is a 2D isometric city-management game developed in Unity.  
The player moves around the city, interacts with plots, constructs or demolishes buildings, and manages city statistics such as housing, employment, food, income, electricity, mental health, and nature.

The goal is to balance these needs and satisfy the win conditions for each level.

## Connection to the Challenge

The game focuses on sustainable city development and is inspired by the United Nations Sustainable Development Goals (SDGs). Each building has benefits and costs. For example, apartments provide housing but increase electricity use and running costs, while parks improve nature and mental health. The player must make trade-offs and build a balanced city. The three levels become progressively more difficult by requiring the player to manage more statistics and stricter targets.

## Controls

### Player
- **W / A / S / D** – Move
- **Space/mouse click** – Interact / Confirm

### Building Menu
- **W / A** – Previous option
- **S / D** – Next option
- **Space** – Select / Confirm

### Navigation
- **Home button** – Return to Main Menu
- **Level buttons** – Select Level 1, 2, or 3

## How to Play

1. Select a level from the Main Menu.
2. Move around the city and approach a plot.
3. Face the plot and press **Space** to interact.
4. Choose a building from the menu and confirm the selection.
5. Buildings can also be demolished and replaced.
6. Check the city statistics and win conditions shown on screen.
7. Continue building until all required conditions are met.

Different buildings affect different statistics, so the player must decide which buildings are needed to complete each level.

## How to Run

### Browser Version
The game can be played directly on itch.io:

**https://bpgg713.itch.io/sustainable-affairs**

### Unity Project
1. Clone or download the repository.
2. Open the `COS30031_Ass2` folder in **Unity 6 LTS**.
3. Open:
   `Assets/Scenes/SceneMainMenu.unity`
4. Press **Play**.

## Key Programming Systems

- **Player Movement and Animation** – Four-direction movement with directional walking and idle animations.

- **Target Plot Detection** – Compares the player's position with nearby plots and uses the player's facing direction to select the target plot.

- **Plot Interaction UI** – Opens the correct building menu for the selected plot.

- **Building Placement and Demolition** – Creates or removes building prefabs on plots and updates the city statistics.

- **City Statistics and Level Completion** – Tracks housing, employment, food, income, costs, electricity, mental health and nature, then checks whether the level requirements have been met.

- **Isometric Sprite Sorting** – Controls whether the player appears in front of or behind buildings based on their positions.

- **2D Collision and Map Boundaries** – Buildings use 2D colliders to stop the player from walking through them, while map boundaries keep the player inside the playable area.

- **Surface Physics** – Different surfaces affect player movement. Roads increase movement speed, water slows the player, and broken roads can create a slippery movement effect.

- **Physics Materials and Debris** – Demolished buildings generate debris using different `PhysicsMaterial2D` settings. Concrete, glass, wood and metal have different friction and bounciness, producing different sliding and bouncing behaviour.

- **Collision Layers** – Player, buildings, debris, surfaces and boundaries use separate collision layers so that only the required objects interact with each other.

- **Main Menu and Scene Navigation** – Provides level selection and a Home button to return to the Main Menu.


## Team Contributions

- **Alexi Davies**: Worked on Informational UI used for tracking each of the game stats and displaying the win conditions. 
- **Ben Pridham**: Worked on stat scripts for keeping track of stats, editing stats when buildings are placed, completion script to monitor if the level is completed, confetti effect on level complete, map layout, game idea/plan.
- **Nho Anh Khoa Nguyen**: Worked on physics and collisions — four physics materials, collision layers and the layer collision matrix, surface speed zones for water, shore, roads and cracked roads across all three levels, map boundaries, and the debris system that spawns material-specific debris when a building is demolished. 
- **Xinzhe Yu**: Worked on player movement and animation, map and player asset integration, target plot detection, plot interaction UI, building placement and demolishment, isometric sorting among builds and player, building collision with player, and the basic Main Menu. 

## Known Issues

No major game-breaking issues are currently known. Minor UI or visual differences may occur depending on browser scaling or screen resolution.


