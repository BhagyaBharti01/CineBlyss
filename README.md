<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cineblyss</title>
    <link rel="stylesheet" href="styles.css"> <!-- Your CSS file -->
</head>
<body>
    <div class="app">
        <header>
            <h1>Cineblyss - Your Movie Night Experience</h1>
        </header>
        
        <!-- Create Room Section -->
        <section id="createRoom">
            <input type="text" id="roomName" placeholder="Enter Room Name" />
            <button id="createRoomBtn">Create Room</button>
        </section>

        <!-- Movie Trivia Section -->
        <section id="movieTrivia" style="display: none;">
            <div id="triviaQuestion">
                <!-- Trivia question and answer will go here -->
            </div>
            <input type="text" id="triviaAnswer" placeholder="Your Answer" />
            <button id="submitTriviaAnswer">Submit Answer</button>
        </section>

        <!-- Movie Reactions Section -->
        <section id="movieReactions" style="display: none;">
            <button class="reactionBtn" onclick="sendReaction('❤️')">❤️</button>
            <button class="reactionBtn" onclick="sendReaction('😂')">😂</button>
            <button class="reactionBtn" onclick="sendReaction('😢')">😢</button>
            <button class="reactionBtn" onclick="sendReaction('😲')">😲</button>
        </section>

        <!-- AI Host Section -->
        <section id="aiHost" style="display: none;">
            <p id="aiMessage">Hello, welcome to Cineblyss! Let's begin your movie night.</p>
            <button onclick="aiResponse()">Talk to Host</button>
        </section>
        
        <footer>
            <p>&copy; 2025 Cineblyss. All rights reserved.</p>
        </footer>
    </div>

    <script src="socket.io.js"></script> <!-- Include Socket.io for real-time features -->
    <script src="app.js"></script> <!-- Your JavaScript logic -->
</body>
</html>
