




    <h1>Simple Game in Scala</h1>
    <h2>Overview</h2>
    <p>This project implements a simple game in Scala where a player navigates a board, collects coins, and avoids walls. The player starts at an initial position and can move around the board to collect points.</p>
    
    <h2>Features</h2>
    <ul>
        <li><strong>10x10 Board</strong>: The game board is a 10x10 grid where each cell can be empty, a wall, or contain a coin.</li>
        <li><strong>Player Movement</strong>: The player can move around the board from an initial position.</li>
        <li><strong>Coins</strong>: Coins are placed at specific positions on the board and have different values.</li>
        <li><strong>Walls</strong>: Certain positions on the board are designated as walls, which the player cannot pass through.</li>
        <li><strong>Score Tracking</strong>: The player's score increases as they collect coins.</li>
    </ul>
    
    <h2>Getting Started</h2>
    <h3>Prerequisites</h3>
    <ul>
        <li>Scala 2.13.x or higher</li>
        <li>sbt (Scala Build Tool)</li>
    </ul>
    
    <h3>Installation</h3>
    <ol>
        <li>Clone the repository:
            <pre><code>git clone https://github.com/your-username/simple-game-scala.git
cd simple-game-scala
            </code></pre>
        </li>
        <li>Compile the project using sbt:
            <pre><code>sbt compile
            </code></pre>
        </li>
        <li>Run the game:
            <pre><code>sbt run
            </code></pre>
        </li>
    </ol>
    
    <h2>Usage</h2>
    <h3>Game Initialization</h3>
    <p>The game is initialized with the following parameters:</p>
    <ul>
        <li><code>wall</code>: A list of coordinates (tuples) where walls exist.</li>
        <li><code>coin</code>: A list of coins, each defined by a position and value (a 3-tuple).</li>
        <li><code>initialX</code>: The initial x position of the player.</li>
        <li><code>initialY</code>: The initial y position of the player.</li>
    </ul>
    <p>Example initialization:</p>
    <pre><code>val game = new Game(
    wall = List((0, 0), (0, 1)),
    coin = List((1, 1, 50), (2, 2, 100)),
    initialX = 0,
    initialY = 0
)
    </code></pre>
    
    <h3>Player Movement</h3>
    <p>The player can move up, down, left, and right. Movement methods and other interactions are defined within the <code>Game</code> class.</p>
    
    <h3>Scoring</h3>
    <p>The player's score is tracked and updated as they collect coins.</p>
    
    <h2>Class Details</h2>
    <h3>Game</h3>
    <p>The <code>Game</code> class holds the instance of the game. Key variables include:</p>
    <ul>
        <li><code>board</code>: A 10x10 grid where -1 represents an empty cell, 0 represents a wall, and positive numbers represent coins.</li>
        <li><code>points</code>: The player's score.</li>
        <li><code>positionX</code> and <code>positionY</code>: The player's current position.</li>
        <li><code>saveX</code> and <code>saveY</code>: Saved positions for the player.</li>
    </ul>
    
    <h3>Methods</h3>
    <p>The <code>Game</code> class includes methods for:</p>
    <ul>
        <li>Initializing the board.</li>
        <li>Moving the player.</li>
        <li>Collecting coins.</li>
        <li>Saving and restoring the player's position.</li>
    </ul>
    
    <h2>Contributing</h2>
    <p>Contributions are welcome! Please create an issue or submit a pull request.</p>
    
    <h2>License</h2>
    <p>This project is licensed under the MIT License. See the <a href="LICENSE">LICENSE</a> file for details.</p>
    
    <h2>Contact</h2>
    <p>For questions or suggestions, please contact <a href="mailto:your-email@example.com">your-email@example.com</a>.</p>
