# -traducteur-universel
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Traducteur Universel</title>
</head>
<body>
    <h1>Bienvenue dans le Traducteur Universel</h1>
    <form>
        <label for="inputText">Entrez votre texte à traduire :</label><br>
        <textarea id="inputText" rows="4" cols="50"></textarea><br><br>
        <button type="button" onclick="translateText()">Traduire</button>
    </form>
    <h2>Texte traduit :</h2>
    <div id="outputText"></div>

    <script>
        function translateText() {
            const input = document.getElementById('inputText').value;
            const output = document.getElementById('outputText');
            // Simuler un traitement de traduction pour cet exemple
            output.innerHTML = 'Traduction du texte : ' + input.split('').reverse().join('');
        }
    </script>
</body>
</html>
