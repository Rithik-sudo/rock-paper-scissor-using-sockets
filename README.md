# 🎮 Multiplayer Rock-Paper-Scissors

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Pygame](https://img.shields.io/badge/Pygame-Ready-green.svg)
![Sockets](https://img.shields.io/badge/Sockets-Networking-orange.svg)

A real-time multiplayer **Rock-Paper-Scissors** game built from scratch using Python, Pygame, and Sockets! This project demonstrates how to build a fully functional networked game where multiple clients connect to a central server and play against each other synchronously.

---

## 📸 Screenshots & UI

Here's what the game looks like in action:

<div align="center">
  <img src="assets/image.png" width="30%" alt="Waiting Screen">
  <img src="assets/image%20copy.png" width="30%" alt="Game Screen">
  <img src="assets/image%20copy%202.png" width="30%" alt="Result Screen">
</div>

---

## 🏗️ Project Architecture

The codebase has been refactored into a clean, modular structure:

- 🖥️ **`server.py`**: The socket server. It pairs incoming client connections, manages the state of each game using the `pickle` module, and orchestrates the matches.
- 🎮 **`client.py`**: The Pygame client application. It handles the graphical user interface, event loops, and rendering.
- 📡 **`network.py`**: The networking logic for the client. It establishes the connection to the server and handles sending/receiving data.
- 🧠 **`game.py`**: The core game logic. It determines match states, validates moves, and calculates winners.

---

## 🚀 How to Run Locally

1. **Start the Server**
   Open a terminal and run the server to start listening for connections:
   ```bash
   python server.py
   ```
   *(You should see "Waiting for a connection, Server Started")*

2. **Start the Clients**
   Open two separate terminal windows and run the client script in each:
   ```bash
   python client.py
   ```
   
3. **Play!**
   The two clients will be automatically paired into a game by the server. Make your moves across the windows and enjoy!

---

## 🎯 Conclusion

In conclusion, our project has successfully implemented a multiplayer Rock-Paper-Scissors game using socket programming, opening the door to real-time gaming experiences. It underscores the potential of networked gaming and the collaborative nature of modern programming. This project offers a starting point for further advancements in online gaming, demonstrating the exciting possibilities of interactive multiplayer experiences in a connected world.

### 🔮 Future Enhancements

1. **Scalability**: Support for more players and concurrent lobbies.
2. **User Authentication**: Accounts and persistent profiles.
3. **Global Chat**: A chat feature for player interaction in the lobby.
4. **Enhanced UI**: Upgraded graphics, animations, and sound effects.
5. **Leaderboards**: Global ranking system for competition.
6. **Game Variations**: Best of 3, Best of 5, or extended rulesets like RPSLS.
7. **Mobile Application**: Porting the networking logic to a mobile framework.
8. **Network Security**: Encrypted socket communication.
9. **AI Opponents**: A fallback single-player mode if no humans are available.
10. **Analytics**: Gameplay statistics, win rates, and history tracking.
11. **Customization**: Player avatars and custom themes.
