# Game Balance Simulator

As a game designer, two of the most important concepts for successful and enjoyable game is iteration and balance. Well designed games constantly iterate over concepts to understand what works well in the game ecosystem and what doesn't. Game balance allows players to experience challenges set upon them by the game or other players in a fair, fun, and engaging way.

While constant iteration and balancing is no issue for larger game development studios, smaller studios and indie developers often lack the extensive amount of time and manpower needed to perform the tedious process of making sure all the numbers and concepts are well balanced. This is especially true at the ideation and concept phase of game design, where rules, mechanics, and general numbers are thought up before a single line of code is written. This issue is exacerbated for physical game developers, who are usually solo designers lacking programming experience.

This project intends to aid smaller game designers to roughly test the balance of their game systems quickly and efficiently, allowing for less time spent iterating through balance updates. While this does not remove the playtesting phase, it may allow designers to identify missable, yet significant weak points in their systems before giving it to testers.

## Major Features

- Graphical interface for user defined variables and scenarios
- Conduct simulations on provided inputs
- Generate statistics and visualizations of simulation results
- Profile import/export for saving and sharing

Stretch goals may include:

- Cloud saving simulations and results
- Account access for cloud saving

## Technologies

This tool will likely use a typical web stack:

- React + TypeScript, Recharts/Chart.js for frontend
- FastAPI for backend
- Python for simulations and strategy logic
- Python + pandas, scipi/statsmodels for statistics
- YAML/JSON for import/export

Technologies for stretch goals:

- SQLite for saving simulations
- JWT for account authentication
- Render/Railway for cloud hosting

## Intended Users

The intended users for this tool are game developers and designers looking for a simple way to test basic mechanical interactions without the need to build a custom simulator. This can especially useful for aspiring game designers who may not have a built up intuition for balancing. These designers may also have simpler systems, making the tool even more effective for balancing these types of games.
