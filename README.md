<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Caricamento Bollette e Dati Utente</title>
    <style>
        body {
            background-image: url('https://scontent.fqpa3-1.fna.fbcdn.net/v/t39.30808-6/398087197_122097271136103429_8513861254678736823_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=5f2048&_nc_ohc=p2jDZJaBmGkAX-ZyjUE&_nc_ht=scontent.fqpa3-1.fna&oh=00_AfBHu8QNzT0oxXKDAxGoIeVb48aDtT1_GRcjiiwGdOSd8g&oe=656114C7');
            background-size: cover;
            background-position: center center;
            color: white;
            padding: 20px;
            height: 100vh;
            margin: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        label,
        input {
            margin-bottom: 10px;
            width: 100%;
        }

        .upload-section {
            margin-bottom: 20px;
            width: 100%;
        }

        button {
            margin-top: 10px;
        }
    </style>
</head>

<body>
    <h1>Caricamento Bollette e Dati Utente</h1>

    <div class="upload-section">
        <h2>Carica la bolletta Luce:</h2>
        <form enctype="multipart/form-data">
            <label for="electricityBillInput">Carica la bolletta (JPG, JPEG, PNG):</label>
            <input type="file" id="electricityBillInput" accept=".jpg, .jpeg, .png" required>
        </form>
    </div>

    <div class="upload-section">
        <h2>Carica la bolletta Gas:</h2>
        <form enctype="multipart/form-data">
            <label for="gasBillInput">Carica la bolletta (JPG, JPEG, PNG):</label>
            <input type="file" id="gasBillInput" accept=".jpg, .jpeg, .png" required>
        </form>
    </div>

    <form>
        <label for="emailInput">Email:</label>
        <input type="email" id="emailInput" required>

        <label for="phoneInput">Numero di cellulare:</label>
        <input type="tel" id="phoneInput" required>

        <label for="idDocumentInput">Documento d'identità:</label>
        <input type="text" id="idDocumentInput" required>

        <label for="ibanInput">IBAN:</label>
        <input type="text" id="ibanInput" required>

        <button type="button" onclick="submitForm()">Invia</button>
    </form>

    <!-- Link a Facebook per recensioni -->
    <p>Se desideri, puoi lasciare una recensione sulla nostra <a href="https://www.facebook.com/profile.php?id=61553102877749" target="_blank">pagina Facebook</a>.</p>

    <script>
        function submitForm() {
            // Implementa la logica per inviare i dati al server
            alert('Dati inviati con successo!');
        }
    </script>
</body>

</html>
