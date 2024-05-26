<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FRANSA SORGU PANELI</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            background: url('https://r.resimlink.com/_vUH0FlAeZ5.jpg') no-repeat center center fixed; /* Fransa'sini buraya koyun */
            background-size: cover;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            font-family: 'Roboto', sans-serif;
        }

        .container {
            background: black;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(255, 255, 255, 0.1);
            width: 100%;
            max-width: 400px;
            text-align: center;
            transition: background-color 1s;
        }

        .container h2 {
            margin-bottom: 20px;
            color: #fff;
            font-family: 'Playfair Display', serif;
            font-weight: 700;
            font-size: 28px;
        }

        .form-group {
            margin-bottom: 20px;
            text-align: left;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            color: #fff;
            font-weight: 700;
            font-size: 16px;
        }

        .form-group input {
            width: 100%;
            padding: 12px;
            border: 2px solid #ccc;
            border-radius: 5px;
            font-size: 16px;
            font-weight: 700;
        }

        .form-group input:focus {
            border-color: #3498db;
            outline: none;
        }

        .btn {
            width: 100%;
            padding: 12px;
            background: blue;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            font-weight: 700;
            cursor: pointer;
            transition: background-color 1s;
        }

        .btn:hover {
            background: darkblue;
        }

        .links {
            margin-top: 20px;
        }

        .links a {
            color: #3498db;
            text-decoration: none;
            font-weight: 700;
            transition: color 0.3s ease;
        }

        .links a:hover {
            color: #2980b9;
        }
    </style>
</head>
<body>
    <div class="container" id="container">
        <h2>FRANSA SORGU PANELİ ONLİNE</h2>
        <form>
            <div class="form-group">
                <label for="email">Kulanıcı</label>
                <input type="email" id="email" required>
            </div>
            <div class="form-group">
                <label for="password">Şifre</label>
                <input type="password" id="password" required>
            </div>
            <button type="submit" class="btn" id="loginButton">Giriş Yap</button>
        </form>
        <div class="links">
            <a href="#"></a>
            <br>
            <a href="#">Kayıt Ol</a>
        </div>
    </div>
    <script>
        const colors = ['black'];

        function changeColors() {
            const container = document.getElementById('container');
            const loginButton = document.getElementById('loginButton');
            const randomColor = colors[Math.floor(Math.random() * colors.length)];

            container.style.backgroundColor = randomColor;
            loginButton.style.backgroundColor = randomColor;
        }

        setInterval(changeColors, 1000);
    </script>
</body>
</html>
