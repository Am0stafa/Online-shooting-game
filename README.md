# Online shooting game

Welcome to the Multiplayer Arena Shooter! Dive into a high-octane battle arena where you and your friends can compete in thrilling team-based combat. Built with Java, this project offers a seamless real-time gaming experience hosted on a local server.

## Table of Contents
- [Getting Started](#getting-started)
- [How It Works](#how-it-works)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Getting Started

These instructions will help you get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Java JDK 8 or later

### Installing

1. Clone the repository:
   ```bash
   git clone https://github.com/Am0stafa/Online-shooting-game.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Online-shooting-game
   ```
3. Compile the Java files:
   ```bash
   javac *.java
   ```
4. Run the server:
   ```bash
   java Server
   ```
5. Run the client(s) on separate terminals or machines:
   ```bash
   java Client
   ```

## How It Works

This game employs Java Swing for GUI rendering and Java Sockets for real-time client-server interaction. Here’s a breakdown of how it operates:

### Networking
- The server continuously listens for new connections, creating a new client handler for each connection to manage communication.
- Utilizing Object Input/Output Streams, complex data structures or custom objects are sent between the server and clients, facilitating detailed game state updates.

### Game State Management
- All game logic is handled on the server side. The server maintains the game state, updating it based on client actions, and sends updates back to the clients at a specified frame rate.
- Clients send their actions to the server, which processes them to update the game state accordingly. The updated state is then sent back to the clients, ensuring a synchronized gaming experience.

### Game Mechanics
- Players can move left, right, jump, and shoot using keyboard controls. The objective is to outscore the opposing team by hitting opponents with bullets while dodging incoming fire and navigating around obstacles.
