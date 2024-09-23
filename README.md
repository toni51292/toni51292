- 👋 Hi, I’m @toni51292
- 👀 I’m interested in football 
- 🌱 I’m currently learning to cook
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Messi vs Ronaldo Abstimmung</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            margin: 20px;
            cursor: pointer;
        }
        .message {
            margin-top: 20px;
            font-weight: bold;
            color: red;
        }
        .results {
            margin-top: 30px;
            font-size: 20px;
            color: green;
        }
        .comments {
            margin-top: 50px;
            text-align: left;
            width: 50%;
            margin: 0 auto;
        }
        .comment {
            background-color: #f0f0f0;
            padding: 10px;
            border-radius: 5px;
            margin-bottom: 10px;
        }
        .scene {
            margin-top: 30px;
        }
        .scene img {
            width: 300px;
            height: auto;
            margin: 20px;
        }
    </style>
</head>
<body>
    <h1>Wer ist der bessere Spieler?</h1>
    <h2>Messi vs Ronaldo</h2>

    <button onclick="vote('messi')">Messi</button>
    <button onclick="vote('ronaldo')">Ronaldo</button>

    <div class="message" id="message"></div>
    <div class="results" id="results"></div>
    <div class="scene" id="scene"></div>
    <div class="comments" id="comments"></div>

    <script>
        const fakeComments = [
            "Ronaldo reitet majestätisch auf einem weißen Pferd in die Geschichte des Fußballs ein.",
            "Messi reitet auf einem strahlend weißen Pferd und erleuchtet das Stadion!",
            "Kein Zweifel, Ronaldo ist der Anführer – er thront auf einem weißen Pferd, während andere nur zusehen können.",
            "Messi auf einem weißen Pferd – wie ein Held, der alle Rekorde bricht!",
            "Ronaldo wird von den Göttern auf einem weißen Pferd durch die Lüfte getragen, während Messi ausgelacht wird.",
            "Messi ist der wahre König – er reitet in den Sonnenuntergang, während die Kindermannschaft Ronaldo auslacht.",
            "Ronaldo auf einem weißen Pferd ist die Definition von Fußball-Eleganz!",
            "Es gibt keinen Spieler, der so episch auf einem weißen Pferd reitet wie Messi!",
            "Während Messi auf einem weißen Pferd durch die Arena reitet, kann Ronaldo nur zusehen.",
            "Ronaldo auf einem weißen Pferd – eine Szene, die man sich in Gold eingravieren könnte.",
            "Messi hat das Spiel auf ein neues Niveau gehoben – er reitet wie ein Ritter auf einem weißen Pferd!",
            "Wenn Messi auf dem Spielfeld ist, sieht man ihn auf einem weißen Pferd durch die Verteidigung reiten.",
            "Ronaldo hebt sich ab – auf einem weißen Pferd, während eine Kindermannschaft Messi auslacht.",
            "Messi wird von allen gefeiert – er reitet auf einem strahlenden weißen Pferd, während Ronaldo hinterherläuft."
        ];

        function vote(player) {
            let chosenPlayer, betterPlayer, chosenImage, betterImage;

            // Festlegen, welcher Spieler gewählt und welcher "besser" ist
            if (player === 'messi') {
                chosenPlayer = 'Messi';
                betterPlayer = 'Ronaldo';
                chosenImage = 'https://example.com/messi_laughed_at.jpg';  // Füge ein Bild hinzu, wie Messi ausgelacht wird
                betterImage = 'https://example.com/ronaldo_on_horse.jpg';  // Füge ein Bild von Ronaldo auf dem Pferd hinzu
            } else {
                chosenPlayer = 'Ronaldo';
                betterPlayer = 'Messi';
                chosenImage = 'https://example.com/ronaldo_laughed_at.jpg';  // Füge ein Bild hinzu, wie Ronaldo ausgelacht wird
                betterImage = 'https://example.com/messi_on_horse.jpg';  // Füge ein Bild von Messi auf dem Pferd hinzu
            }

            // Nachricht anzeigen
            document.getElementById('message').innerText = `Du hast für ${chosenPlayer} gestimmt. Leider bist du minderbemittelt.`;

            // Ergebnisanzeige manipulieren (100% für den anderen Spieler)
            document.getElementById('results').innerText = `100% der bisherigen Nutzer haben für ${betterPlayer} gestimmt. Du bist die erste Person, die für ${chosenPlayer} stimmt.`;

            // Szenen anzeigen (weißer Reiter vs. Kindermannschaft, die lacht)
            document.getElementById('scene').innerHTML = `
                <img src="${betterImage}" alt="${betterPlayer} auf einem weißen Pferd">
                <img src="${chosenImage}" alt="${chosenPlayer} wird von einer Kindermannschaft ausgelacht">
            `;

            // Fake-Kommentare anzeigen
            displayComments(betterPlayer);
        }

        function displayComments(betterPlayer) {
            const commentsDiv = document.getElementById('comments');
            commentsDiv.innerHTML = '';  // Alle vorherigen Kommentare entfernen

            // Generiere zufällige Fake-Kommentare
            fakeComments.forEach(comment => {
                const commentDiv = document.createElement('div');
                commentDiv.className = 'comment';
                commentDiv.innerText = comment.replace(/Messi|Ronaldo/g, betterPlayer);  // Passe den Namen des besseren Spielers an
                commentsDiv.appendChild(commentDiv);
            });
        }
    </script>
</body>
</html>!---
toni51292/toni51292 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
