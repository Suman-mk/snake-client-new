# snake-client

Snake game is a very popular video game. It is a video game concept where the player maneuvers a dot and grows it by ‘eating’ pieces of food. As it moves and eats, it grows and the growing snake becomes an obstacle to smooth maneuvers. The goal is to grow it to become as big as possible without bumping into the side walls, or bumping into itself, upon which it dies.

This is simply a multiplayer take on the genre.

Before you can run this client, you will need to be running the server side which you can download and install from here. 
git clone https://github.com/lighthouse-labs/snek-multiplayer.git
cd snek-multiplayer
npm install
npm run play
[
IP: 192.168.2.27 
PORT: 50541 
]
      

## Getting Started

- Follow steps inside the snek server repo to run the server side
- Run the development snake client using the `node play.js` command.

play.js
Establishes connection to the server.

input.js
Handles all the logic related to setting up input stream and handling user input.

client.js
Establishes connection to the server- for the localhost. Prints Connected to server... upon successful connection. Sets the snake-name to SM upon successful connection. Logs server responses to screen.

logger.js
Universal logger used throughout this application. Currently console.log is used to prinnt to the console.


Supported commands by Snek-Multiplayer server
Commands are passed by as utf8 strings between client and server. Name: SM

Sets the name for snake; in this case SM is the desired name name.
 Move: up
Moves the snake up one block, (unless facing down) Move: down
Moves the snake down one block, (unless facing up) Move: left
Moves the snake left one block, (unless facing right) Move: right
Moves the snake right one block, (unless facing left) Say: {hi there}
Short chat message to be displayed on the screen; in this case {hi there}.

Handles all the logic related to setting up input stream and handling user input.

Key	Command
W , w , '8'	  sends move up command
A , a , '4'	  sends move left command
S , s , '2'	  sends move down command
D , d , '6'	  sends move right command
H, h	        sends canned message 'Hi there'
B, b	        sends canned message 'Bye ppl'
G, g	        sends canned message 'Got to go'