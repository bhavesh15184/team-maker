# A simple HTML page to create teams from a group of players. It uses the skill points assigned to players to distribute them into teams equally. For now, this is used to create Vollyball teams but its easily extendable to other sports.

# Interactive Table with Edit, Add, and Delete

This project provides an interactive HTML table that allows users to manage a list of players, including their names, availability, and skill points. It also features functionality to dynamically distribute players into teams based on their skill points and to sort the players' list.

## Features

- **Add New Player**: Users can add a new player by entering their name, selecting their availability, and assigning skill points.
- **Delete Player**: Users can delete a player from the list.
- **Sort Players**: The table supports sorting by clicking on the column headers. It can sort both text and numeric columns.
- **Distribute Players into Teams**: Based on the players' skill points, the application distributes players into teams, ensuring a balanced distribution according to predefined rules.
- **Dynamic Team Table Generation**: The application dynamically generates a team table displaying the distribution of players into teams, including the total skill points per team.

## How It Works

1. **Pre-population of Players**: Upon loading, the table is pre-populated with a set of predefined players.
2. **Adding a Row**: Users can add a new player by clicking the "Add Row" button, which prompts input fields for the player's details.
3. **Deleting a Row**: Each row has a "Delete" button, allowing users to remove the player from the list.
4. **Sorting**: Clicking on a column header sorts the players based on that column. The sort direction toggles between ascending and descending.
5. **Distributing Players**: Clicking the "Regenerate Teams" button triggers the distribution of players into teams based on their skill points, updating the Teams table accordingly.

## Implementation Details

- The application is implemented in plain HTML and JavaScript, demonstrating DOM manipulation and event handling.
- Sorting functionality is implemented to handle both numeric and text-based sorting, with visual indicators for sort direction.
- Team distribution takes into account the number of players and their skill points to evenly distribute players into an appropriate number of teams.

## Setup

To run this project, simply open the `test.html` file in a web browser. No additional setup or dependencies are required.

## Limitations

- This project is created within a single HTML with JS code in it. So that people can run it on mobile phone browser without a need of native app.
- The current implementation assumes a static set of skill points (1-10) and does not support custom skill levels.
- The team distribution algorithm is basic and does not account for more complex balancing factors beyond skill points.

## Future Enhancements

- Enhancing the team distribution algorithm to account for more nuanced balancing factors.
- Adding functionality to edit existing player entries directly within the table.
- Implementing persistent storage of player data using local storage or a backend service.