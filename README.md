<!DOCTYPE html>
<html>
<head>
    <title>Random Task Generator</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; padding: 50px; }
        #task { font-size: 24px; margin: 20px; }
        button { padding: 10px 20px; font-size: 18px; cursor: pointer; }
    </style>
</head>
<body>
    <h1>Random Task Generator</h1>
    <p>Click the button to get your task for the day!</p>
    <button onclick="generateTask()">Generate Task</button>
    <p id="task"></p>
    
    <script>
        const tasks = [
            "Try a new snooker trick shot",
            "Read a random page from a self-improvement book & apply it",
            "Test a new AI tool for content creation",
            "Cook something you’ve never made before",
            "Do a workout you’ve never tried",
            "Meditate in silence for 30 minutes & share insights",
            "Record a voice-over with a different tone or accent",
            "Go to a random place & interact with strangers",
            "Write a blog post using only AI suggestions",
            "Listen to a random song & analyze its lyrics deeply"
        ];
        
        function generateTask() {
            const randomIndex = Math.floor(Math.random() * tasks.length);
            document.getElementById("task").innerText = tasks[randomIndex];
        }
    </script>
</body>
</html>
