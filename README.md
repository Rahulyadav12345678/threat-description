<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>National Security Threat Assessment Tool</title>
    <link rel="stylesheet" href="style.css">
    <style>
        body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background-color: #333;
    color: white;
    padding: 20px;
    text-align: center;
}

.input-section, .result-section {
    margin: 20px auto;
    max-width: 800px;
    background-color: white;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h2 {
    margin-top: 0;
}

form {
    display: flex;
    flex-direction: column;
}

label {
    margin: 10px 0 5px;
}

textarea, select {
    padding: 10px;
    font-size: 1rem;
    margin-bottom: 15px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

button {
    padding: 10px;
    background-color: #333;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
}

button:hover {
    background-color: #555;
}

.result-section ul {
    list-style: none;
    padding: 0;
}

.result-section li {
    background-color: #e2e2e2;
    padding: 10px;
    margin-bottom: 10px;
    border-radius: 5px;
}

    </style>
</head>
<body>
    <header>
        <h1>National Security Threat Assessment Tool</h1>
    </header>

    <section class="input-section">
        <h2>Evaluate a Threat</h2>
        <form id="threat-form">
            <label for="threat-description">Threat Description:</label>
            <textarea id="threat-description" placeholder="Describe the threat..." required></textarea>

            <label for="threat-level">Risk Level:</label>
            <select id="threat-level" required>
                <option value="Low">Low</option>
                <option value="Medium">Medium</option>
                <option value="High">High</option>
            </select>

            <label for="threat-category">Category:</label>
            <select id="threat-category" required>
                <option value="Cybersecurity">Cybersecurity</option>
                <option value="Terrorism">Terrorism</option>
                <option value="Biological">Biological</option>
                <option value="Natural Disaster">Natural Disaster</option>
                <option value="Other">Other</option>
            </select>

            <button type="submit">Assess Threat</button>
        </form>
    </section>

    <section class="result-section">
        <h2>Threat Assessment Results</h2>
        <ul id="threat-results"></ul>
    </section>

    <script src="script.js"></script>
</body>
</html>
